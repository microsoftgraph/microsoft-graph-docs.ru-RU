# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="9ea6c-101">Тип ресурса deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="9ea6c-101">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="9ea6c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9ea6c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ea6c-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9ea6c-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="9ea6c-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ea6c-104">Properties</span></span>
|<span data-ttu-id="9ea6c-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ea6c-105">Property</span></span>|<span data-ttu-id="9ea6c-106">Тип</span><span class="sxs-lookup"><span data-stu-id="9ea6c-106">Type</span></span>|<span data-ttu-id="9ea6c-107">Описание</span><span class="sxs-lookup"><span data-stu-id="9ea6c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ea6c-108">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="9ea6c-108">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="9ea6c-109">Int32</span><span class="sxs-lookup"><span data-stu-id="9ea6c-109">Int32</span></span>|<span data-ttu-id="9ea6c-110">Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.</span><span class="sxs-lookup"><span data-stu-id="9ea6c-110">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="9ea6c-111">Допустимые значения: от 0 до 120</span><span class="sxs-lookup"><span data-stu-id="9ea6c-111">Valid values 0 to 120</span></span>|
|<span data-ttu-id="9ea6c-112">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="9ea6c-112">isScheduledActionEnabled</span></span>|<span data-ttu-id="9ea6c-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ea6c-113">Boolean</span></span>|<span data-ttu-id="9ea6c-114">Включена ли функция для запланированного действия для правила.</span><span class="sxs-lookup"><span data-stu-id="9ea6c-114">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="9ea6c-115">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="9ea6c-115">secureByDefault</span></span>|<span data-ttu-id="9ea6c-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ea6c-116">Boolean</span></span>|<span data-ttu-id="9ea6c-117">Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="9ea6c-117">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ea6c-118">Связи</span><span class="sxs-lookup"><span data-stu-id="9ea6c-118">Relationships</span></span>
<span data-ttu-id="9ea6c-119">Нет</span><span class="sxs-lookup"><span data-stu-id="9ea6c-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9ea6c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9ea6c-120">JSON Representation</span></span>
<span data-ttu-id="9ea6c-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ea6c-121">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true
}
```








