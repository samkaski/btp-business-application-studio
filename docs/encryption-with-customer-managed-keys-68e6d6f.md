<!-- loio68e6d6f7b8f6436e986214e79cb7bf9c -->

# Encryption with Customer-Managed Keys

SAP Business Application Studio supports customer-managed keys \(CMK\) to encrypt files and folders.

CMK functionality is enabled by default for all dev spaces that were created from September 18, 2022 and onwards:

-   For all files and folders in your dev space, located under `/home/user`, the data is persisted in the physical storage in encrypted form. Access to the files and folders requires the CMK key to be enabled in the SAP Key Management Service \(KMS\), which is the default case.
-   If you opt to disable the managed keys, then dev spaces in your tenant won’t be able to start and new dev spaces can’t be created. As long as the managed keys are disabled, the files will not be accessible by SAP Business Application Studio components. Existing dev spaces will be reachable again when you enable the managed keys.
