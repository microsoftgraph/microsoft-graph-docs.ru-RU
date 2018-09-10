# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="c90cf-101">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="c90cf-101">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="c90cf-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c90cf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c90cf-103">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="c90cf-103">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="c90cf-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="c90cf-104">Properties</span></span>
|<span data-ttu-id="c90cf-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="c90cf-105">Property</span></span>|<span data-ttu-id="c90cf-106">Тип</span><span class="sxs-lookup"><span data-stu-id="c90cf-106">Type</span></span>|<span data-ttu-id="c90cf-107">Описание</span><span class="sxs-lookup"><span data-stu-id="c90cf-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c90cf-108">validationName</span><span class="sxs-lookup"><span data-stu-id="c90cf-108">validationName</span></span>|<span data-ttu-id="c90cf-109">String</span><span class="sxs-lookup"><span data-stu-id="c90cf-109">String</span></span>|<span data-ttu-id="c90cf-110">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="c90cf-110">The validation friendly name</span></span>|
|<span data-ttu-id="c90cf-111">state</span><span class="sxs-lookup"><span data-stu-id="c90cf-111">state</span></span>|<span data-ttu-id="c90cf-112">String</span><span class="sxs-lookup"><span data-stu-id="c90cf-112">String</span></span>|<span data-ttu-id="c90cf-113">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="c90cf-113">The state of the operation</span></span>|
|<span data-ttu-id="c90cf-114">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="c90cf-114">mitigationInstruction</span></span>|<span data-ttu-id="c90cf-115">String</span><span class="sxs-lookup"><span data-stu-id="c90cf-115">String</span></span>|<span data-ttu-id="c90cf-116">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="c90cf-116">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="c90cf-117">Связи</span><span class="sxs-lookup"><span data-stu-id="c90cf-117">Relationships</span></span>
<span data-ttu-id="c90cf-118">Нет</span><span class="sxs-lookup"><span data-stu-id="c90cf-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c90cf-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c90cf-119">JSON Representation</span></span>
<span data-ttu-id="c90cf-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c90cf-120">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```








