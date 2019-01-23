---
title: Тип ресурса mobileAppTroubleshootingAppPolicyCreationHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e81f7f39cac934a89cf06d77fbcb80581267097b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394560"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="48fbb-103">Тип ресурса mobileAppTroubleshootingAppPolicyCreationHistory</span><span class="sxs-lookup"><span data-stu-id="48fbb-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="48fbb-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="48fbb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="48fbb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48fbb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48fbb-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48fbb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48fbb-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="48fbb-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="48fbb-108">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="48fbb-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="48fbb-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="48fbb-109">Properties</span></span>
|<span data-ttu-id="48fbb-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="48fbb-110">Property</span></span>|<span data-ttu-id="48fbb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="48fbb-111">Type</span></span>|<span data-ttu-id="48fbb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="48fbb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48fbb-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="48fbb-113">occurrenceDateTime</span></span>|<span data-ttu-id="48fbb-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48fbb-114">DateTimeOffset</span></span>|<span data-ttu-id="48fbb-115">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="48fbb-115">Time when the history item occurred.</span></span> <span data-ttu-id="48fbb-116">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="48fbb-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="48fbb-117">runState</span><span class="sxs-lookup"><span data-stu-id="48fbb-117">runState</span></span>|[<span data-ttu-id="48fbb-118">runState</span><span class="sxs-lookup"><span data-stu-id="48fbb-118">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="48fbb-119">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="48fbb-119">Status of the item.</span></span> <span data-ttu-id="48fbb-120">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="48fbb-120">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="48fbb-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="48fbb-121">errorCode</span></span>|<span data-ttu-id="48fbb-122">String</span><span class="sxs-lookup"><span data-stu-id="48fbb-122">String</span></span>|<span data-ttu-id="48fbb-123">Код ошибки сбоя, пустой, если нет сбоев.</span><span class="sxs-lookup"><span data-stu-id="48fbb-123">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48fbb-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="48fbb-124">Relationships</span></span>
<span data-ttu-id="48fbb-125">Нет</span><span class="sxs-lookup"><span data-stu-id="48fbb-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48fbb-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="48fbb-126">JSON Representation</span></span>
<span data-ttu-id="48fbb-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48fbb-127">Here is a JSON representation of the resource.</span></span>
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




