---
title: Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 416a5c7171a03db48d0b349a2a6415a940e5b798
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988071"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="38aef-103">Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори</span><span class="sxs-lookup"><span data-stu-id="38aef-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="38aef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38aef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38aef-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38aef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38aef-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="38aef-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="38aef-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="38aef-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="38aef-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="38aef-108">Properties</span></span>
|<span data-ttu-id="38aef-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="38aef-109">Property</span></span>|<span data-ttu-id="38aef-110">Тип</span><span class="sxs-lookup"><span data-stu-id="38aef-110">Type</span></span>|<span data-ttu-id="38aef-111">Описание</span><span class="sxs-lookup"><span data-stu-id="38aef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38aef-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="38aef-112">occurrenceDateTime</span></span>|<span data-ttu-id="38aef-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38aef-113">DateTimeOffset</span></span>|<span data-ttu-id="38aef-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="38aef-114">Time when the history item occurred.</span></span> <span data-ttu-id="38aef-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="38aef-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="38aef-116">Рунстате</span><span class="sxs-lookup"><span data-stu-id="38aef-116">runState</span></span>|[<span data-ttu-id="38aef-117">Рунстате</span><span class="sxs-lookup"><span data-stu-id="38aef-117">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="38aef-118">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="38aef-118">Status of the item.</span></span> <span data-ttu-id="38aef-119">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="38aef-119">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="38aef-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="38aef-120">errorCode</span></span>|<span data-ttu-id="38aef-121">String</span><span class="sxs-lookup"><span data-stu-id="38aef-121">String</span></span>|<span data-ttu-id="38aef-122">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="38aef-122">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38aef-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="38aef-123">Relationships</span></span>
<span data-ttu-id="38aef-124">Нет</span><span class="sxs-lookup"><span data-stu-id="38aef-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38aef-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38aef-125">JSON Representation</span></span>
<span data-ttu-id="38aef-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38aef-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory",
  "occurrenceDateTime": "String (timestamp)",
  "runState": "String",
  "errorCode": "String"
}
```





