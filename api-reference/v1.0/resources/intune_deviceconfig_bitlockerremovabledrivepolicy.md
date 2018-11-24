# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="4de85-101">Тип ресурса bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="4de85-101">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="4de85-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4de85-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4de85-103">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="4de85-103">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="4de85-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="4de85-104">Properties</span></span>
|<span data-ttu-id="4de85-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="4de85-105">Property</span></span>|<span data-ttu-id="4de85-106">Тип</span><span class="sxs-lookup"><span data-stu-id="4de85-106">Type</span></span>|<span data-ttu-id="4de85-107">Описание</span><span class="sxs-lookup"><span data-stu-id="4de85-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4de85-108">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="4de85-108">encryptionMethod</span></span>|[<span data-ttu-id="4de85-109">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="4de85-109">bitLockerEncryptionMethod</span></span>](../resources/intune_deviceconfig_bitlockerencryptionmethod.md)|<span data-ttu-id="4de85-110">Выберите метод шифрования для съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="4de85-110">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="4de85-111">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="4de85-111">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="4de85-112">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="4de85-112">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="4de85-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="4de85-113">Boolean</span></span>|<span data-ttu-id="4de85-114">Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.</span><span class="sxs-lookup"><span data-stu-id="4de85-114">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="4de85-115">Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.</span><span class="sxs-lookup"><span data-stu-id="4de85-115">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="4de85-116">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="4de85-116">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="4de85-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="4de85-117">Boolean</span></span>|<span data-ttu-id="4de85-118">Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="4de85-118">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4de85-119">Связи</span><span class="sxs-lookup"><span data-stu-id="4de85-119">Relationships</span></span>
<span data-ttu-id="4de85-120">Нет</span><span class="sxs-lookup"><span data-stu-id="4de85-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4de85-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4de85-121">JSON Representation</span></span>
<span data-ttu-id="4de85-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4de85-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```



