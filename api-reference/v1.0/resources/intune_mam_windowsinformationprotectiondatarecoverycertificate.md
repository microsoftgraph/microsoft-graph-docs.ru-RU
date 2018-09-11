# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="27f1b-101">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="27f1b-101">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="27f1b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="27f1b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27f1b-103">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="27f1b-103">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="27f1b-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="27f1b-104">Properties</span></span>
|<span data-ttu-id="27f1b-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="27f1b-105">Property</span></span>|<span data-ttu-id="27f1b-106">Тип</span><span class="sxs-lookup"><span data-stu-id="27f1b-106">Type</span></span>|<span data-ttu-id="27f1b-107">Описание</span><span class="sxs-lookup"><span data-stu-id="27f1b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27f1b-108">subjectName</span><span class="sxs-lookup"><span data-stu-id="27f1b-108">subjectName</span></span>|<span data-ttu-id="27f1b-109">Строка</span><span class="sxs-lookup"><span data-stu-id="27f1b-109">String</span></span>|<span data-ttu-id="27f1b-110">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="27f1b-110">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="27f1b-111">описание</span><span class="sxs-lookup"><span data-stu-id="27f1b-111">description</span></span>|<span data-ttu-id="27f1b-112">Строка</span><span class="sxs-lookup"><span data-stu-id="27f1b-112">String</span></span>|<span data-ttu-id="27f1b-113">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="27f1b-113">Data recovery Certificate description</span></span>|
|<span data-ttu-id="27f1b-114">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="27f1b-114">expirationDateTime</span></span>|<span data-ttu-id="27f1b-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27f1b-115">DateTimeOffset</span></span>|<span data-ttu-id="27f1b-116">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="27f1b-116">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="27f1b-117">сертификат</span><span class="sxs-lookup"><span data-stu-id="27f1b-117">certificate</span></span>|<span data-ttu-id="27f1b-118">Двоичный</span><span class="sxs-lookup"><span data-stu-id="27f1b-118">Binary</span></span>|<span data-ttu-id="27f1b-119">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="27f1b-119">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="27f1b-120">Связи</span><span class="sxs-lookup"><span data-stu-id="27f1b-120">Relationships</span></span>
<span data-ttu-id="27f1b-121">Нет</span><span class="sxs-lookup"><span data-stu-id="27f1b-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="27f1b-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27f1b-122">JSON Representation</span></span>
<span data-ttu-id="27f1b-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27f1b-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```








