# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="479d9-101">Тип ресурса bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="479d9-101">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="479d9-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="479d9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="479d9-103">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="479d9-103">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="479d9-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="479d9-104">Properties</span></span>
|<span data-ttu-id="479d9-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="479d9-105">Property</span></span>|<span data-ttu-id="479d9-106">Тип</span><span class="sxs-lookup"><span data-stu-id="479d9-106">Type</span></span>|<span data-ttu-id="479d9-107">Описание</span><span class="sxs-lookup"><span data-stu-id="479d9-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="479d9-108">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="479d9-108">encryptionMethod</span></span>|<span data-ttu-id="479d9-109">String</span><span class="sxs-lookup"><span data-stu-id="479d9-109">String</span></span>|<span data-ttu-id="479d9-110">Выберите метод шифрования для съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="479d9-110">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="479d9-111">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="479d9-111">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="479d9-112">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="479d9-112">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="479d9-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="479d9-113">Boolean</span></span>|<span data-ttu-id="479d9-114">Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.</span><span class="sxs-lookup"><span data-stu-id="479d9-114">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="479d9-115">Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.</span><span class="sxs-lookup"><span data-stu-id="479d9-115">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="479d9-116">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="479d9-116">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="479d9-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="479d9-117">Boolean</span></span>|<span data-ttu-id="479d9-118">Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="479d9-118">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="479d9-119">Связи</span><span class="sxs-lookup"><span data-stu-id="479d9-119">Relationships</span></span>
<span data-ttu-id="479d9-120">Нет</span><span class="sxs-lookup"><span data-stu-id="479d9-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="479d9-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="479d9-121">JSON Representation</span></span>
<span data-ttu-id="479d9-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="479d9-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



