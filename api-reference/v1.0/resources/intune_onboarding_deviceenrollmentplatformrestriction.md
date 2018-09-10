# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="d5d15-101">Тип ресурса deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d5d15-101">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="d5d15-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d5d15-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5d15-103">Ограничения на регистрацию для определенных платформ</span><span class="sxs-lookup"><span data-stu-id="d5d15-103">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="d5d15-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="d5d15-104">Properties</span></span>
|<span data-ttu-id="d5d15-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5d15-105">Property</span></span>|<span data-ttu-id="d5d15-106">Тип</span><span class="sxs-lookup"><span data-stu-id="d5d15-106">Type</span></span>|<span data-ttu-id="d5d15-107">Описание</span><span class="sxs-lookup"><span data-stu-id="d5d15-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5d15-108">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="d5d15-108">platformBlocked</span></span>|<span data-ttu-id="d5d15-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5d15-109">Boolean</span></span>|<span data-ttu-id="d5d15-110">Указывает, блокируется ли регистрация платформы</span><span class="sxs-lookup"><span data-stu-id="d5d15-110">Block the platform from enrolling</span></span>|
|<span data-ttu-id="d5d15-111">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="d5d15-111">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="d5d15-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5d15-112">Boolean</span></span>|<span data-ttu-id="d5d15-113">Указывает, блокируется ли регистрация личных устройств</span><span class="sxs-lookup"><span data-stu-id="d5d15-113">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="d5d15-114">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="d5d15-114">osMinimumVersion</span></span>|<span data-ttu-id="d5d15-115">String</span><span class="sxs-lookup"><span data-stu-id="d5d15-115">String</span></span>|<span data-ttu-id="d5d15-116">Минимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="d5d15-116">Min OS version supported</span></span>|
|<span data-ttu-id="d5d15-117">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="d5d15-117">osMaximumVersion</span></span>|<span data-ttu-id="d5d15-118">String</span><span class="sxs-lookup"><span data-stu-id="d5d15-118">String</span></span>|<span data-ttu-id="d5d15-119">Максимальная поддерживаемая версия ОС</span><span class="sxs-lookup"><span data-stu-id="d5d15-119">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5d15-120">Связи</span><span class="sxs-lookup"><span data-stu-id="d5d15-120">Relationships</span></span>
<span data-ttu-id="d5d15-121">Нет</span><span class="sxs-lookup"><span data-stu-id="d5d15-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d5d15-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d5d15-122">JSON Representation</span></span>
<span data-ttu-id="d5d15-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5d15-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```








