---
title: Тип ресурса mobileAppTroubleshootingAppPolicyCreationHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
ms.openlocfilehash: 7ca80443351e5c1b1232dc050cdf721ab7389351
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081131"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="067a1-103">Тип ресурса mobileAppTroubleshootingAppPolicyCreationHistory</span><span class="sxs-lookup"><span data-stu-id="067a1-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="067a1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="067a1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="067a1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="067a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="067a1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="067a1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="067a1-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="067a1-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="067a1-108">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="067a1-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="067a1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="067a1-109">Properties</span></span>
|<span data-ttu-id="067a1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="067a1-110">Property</span></span>|<span data-ttu-id="067a1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="067a1-111">Type</span></span>|<span data-ttu-id="067a1-112">Description</span><span class="sxs-lookup"><span data-stu-id="067a1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="067a1-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="067a1-113">occurrenceDateTime</span></span>|<span data-ttu-id="067a1-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="067a1-114">DateTimeOffset</span></span>|<span data-ttu-id="067a1-115">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="067a1-115">Time when the history item occurred.</span></span> <span data-ttu-id="067a1-116">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="067a1-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="067a1-117">runState</span><span class="sxs-lookup"><span data-stu-id="067a1-117">runState</span></span>|[<span data-ttu-id="067a1-118">runState</span><span class="sxs-lookup"><span data-stu-id="067a1-118">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="067a1-119">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="067a1-119">Status of the item.</span></span> <span data-ttu-id="067a1-120">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="067a1-120">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="067a1-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="067a1-121">errorCode</span></span>|<span data-ttu-id="067a1-122">String</span><span class="sxs-lookup"><span data-stu-id="067a1-122">String</span></span>|<span data-ttu-id="067a1-123">Код ошибки сбоя, пустой, если нет сбоев.</span><span class="sxs-lookup"><span data-stu-id="067a1-123">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="067a1-124">Связи</span><span class="sxs-lookup"><span data-stu-id="067a1-124">Relationships</span></span>
<span data-ttu-id="067a1-125">Нет</span><span class="sxs-lookup"><span data-stu-id="067a1-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="067a1-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="067a1-126">JSON Representation</span></span>
<span data-ttu-id="067a1-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="067a1-127">Here is a JSON representation of the resource.</span></span>
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





