---
title: Тип ресурса mobileAppTroubleshootingAppPolicyCreationHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0ee2088856c9c47771b3e647615f82fe26dfd552
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924393"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="08ffc-103">Тип ресурса mobileAppTroubleshootingAppPolicyCreationHistory</span><span class="sxs-lookup"><span data-stu-id="08ffc-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="08ffc-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="08ffc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08ffc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08ffc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08ffc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="08ffc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08ffc-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="08ffc-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="08ffc-108">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="08ffc-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="08ffc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="08ffc-109">Properties</span></span>
|<span data-ttu-id="08ffc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="08ffc-110">Property</span></span>|<span data-ttu-id="08ffc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="08ffc-111">Type</span></span>|<span data-ttu-id="08ffc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="08ffc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08ffc-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="08ffc-113">occurrenceDateTime</span></span>|<span data-ttu-id="08ffc-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08ffc-114">DateTimeOffset</span></span>|<span data-ttu-id="08ffc-115">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="08ffc-115">Time when the history item occurred.</span></span> <span data-ttu-id="08ffc-116">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="08ffc-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="08ffc-117">runState</span><span class="sxs-lookup"><span data-stu-id="08ffc-117">runState</span></span>|[<span data-ttu-id="08ffc-118">runState</span><span class="sxs-lookup"><span data-stu-id="08ffc-118">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="08ffc-119">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="08ffc-119">Status of the item.</span></span> <span data-ttu-id="08ffc-120">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="08ffc-120">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="08ffc-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="08ffc-121">errorCode</span></span>|<span data-ttu-id="08ffc-122">String</span><span class="sxs-lookup"><span data-stu-id="08ffc-122">String</span></span>|<span data-ttu-id="08ffc-123">Код ошибки сбоя, пустой, если нет сбоев.</span><span class="sxs-lookup"><span data-stu-id="08ffc-123">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08ffc-124">Связи</span><span class="sxs-lookup"><span data-stu-id="08ffc-124">Relationships</span></span>
<span data-ttu-id="08ffc-125">Нет</span><span class="sxs-lookup"><span data-stu-id="08ffc-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="08ffc-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08ffc-126">JSON Representation</span></span>
<span data-ttu-id="08ffc-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08ffc-127">Here is a JSON representation of the resource.</span></span>
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





