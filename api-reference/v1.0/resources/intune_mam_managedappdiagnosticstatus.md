# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="f150c-101">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="f150c-101">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="f150c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f150c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f150c-103">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="f150c-103">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="f150c-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="f150c-104">Properties</span></span>
|<span data-ttu-id="f150c-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="f150c-105">Property</span></span>|<span data-ttu-id="f150c-106">Тип</span><span class="sxs-lookup"><span data-stu-id="f150c-106">Type</span></span>|<span data-ttu-id="f150c-107">Описание</span><span class="sxs-lookup"><span data-stu-id="f150c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f150c-108">validationName</span><span class="sxs-lookup"><span data-stu-id="f150c-108">validationName</span></span>|<span data-ttu-id="f150c-109">String</span><span class="sxs-lookup"><span data-stu-id="f150c-109">String</span></span>|<span data-ttu-id="f150c-110">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="f150c-110">The validation friendly name</span></span>|
|<span data-ttu-id="f150c-111">state</span><span class="sxs-lookup"><span data-stu-id="f150c-111">state</span></span>|<span data-ttu-id="f150c-112">String</span><span class="sxs-lookup"><span data-stu-id="f150c-112">String</span></span>|<span data-ttu-id="f150c-113">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="f150c-113">The state of the operation</span></span>|
|<span data-ttu-id="f150c-114">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="f150c-114">mitigationInstruction</span></span>|<span data-ttu-id="f150c-115">String</span><span class="sxs-lookup"><span data-stu-id="f150c-115">String</span></span>|<span data-ttu-id="f150c-116">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="f150c-116">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="f150c-117">Связи</span><span class="sxs-lookup"><span data-stu-id="f150c-117">Relationships</span></span>
<span data-ttu-id="f150c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f150c-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f150c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f150c-119">JSON Representation</span></span>
<span data-ttu-id="f150c-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f150c-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```



