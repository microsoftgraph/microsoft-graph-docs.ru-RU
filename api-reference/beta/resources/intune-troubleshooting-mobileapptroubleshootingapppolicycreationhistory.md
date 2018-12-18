---
title: Тип ресурса mobileAppTroubleshootingAppPolicyCreationHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
author: tfitzmac
ms.openlocfilehash: 6d0192e8dde3cfc858629f7ae79e4b7de786740a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301458"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="d0d96-103">Тип ресурса mobileAppTroubleshootingAppPolicyCreationHistory</span><span class="sxs-lookup"><span data-stu-id="d0d96-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="d0d96-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d0d96-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0d96-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0d96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0d96-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d0d96-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0d96-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="d0d96-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="d0d96-108">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d0d96-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d0d96-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0d96-109">Properties</span></span>
|<span data-ttu-id="d0d96-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0d96-110">Property</span></span>|<span data-ttu-id="d0d96-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d0d96-111">Type</span></span>|<span data-ttu-id="d0d96-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d0d96-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0d96-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="d0d96-113">occurrenceDateTime</span></span>|<span data-ttu-id="d0d96-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0d96-114">DateTimeOffset</span></span>|<span data-ttu-id="d0d96-115">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="d0d96-115">Time when the history item occurred.</span></span> <span data-ttu-id="d0d96-116">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d0d96-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="d0d96-117">runState</span><span class="sxs-lookup"><span data-stu-id="d0d96-117">runState</span></span>|[<span data-ttu-id="d0d96-118">runState</span><span class="sxs-lookup"><span data-stu-id="d0d96-118">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="d0d96-119">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="d0d96-119">Status of the item.</span></span> <span data-ttu-id="d0d96-120">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="d0d96-120">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="d0d96-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="d0d96-121">errorCode</span></span>|<span data-ttu-id="d0d96-122">String</span><span class="sxs-lookup"><span data-stu-id="d0d96-122">String</span></span>|<span data-ttu-id="d0d96-123">Код ошибки сбоя, пустой, если нет сбоев.</span><span class="sxs-lookup"><span data-stu-id="d0d96-123">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0d96-124">Связи</span><span class="sxs-lookup"><span data-stu-id="d0d96-124">Relationships</span></span>
<span data-ttu-id="d0d96-125">Нет</span><span class="sxs-lookup"><span data-stu-id="d0d96-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d0d96-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0d96-126">JSON Representation</span></span>
<span data-ttu-id="d0d96-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0d96-127">Here is a JSON representation of the resource.</span></span>
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





