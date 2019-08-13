---
title: Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6df5367e0c52c7db32c840dcd5b0cf9255e6e289
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372855"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="0b5b6-103">Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори</span><span class="sxs-lookup"><span data-stu-id="0b5b6-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="0b5b6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b5b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b5b6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b5b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b5b6-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="0b5b6-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="0b5b6-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="0b5b6-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0b5b6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b5b6-108">Properties</span></span>
|<span data-ttu-id="0b5b6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b5b6-109">Property</span></span>|<span data-ttu-id="0b5b6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0b5b6-110">Type</span></span>|<span data-ttu-id="0b5b6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0b5b6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b5b6-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="0b5b6-112">occurrenceDateTime</span></span>|<span data-ttu-id="0b5b6-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b5b6-113">DateTimeOffset</span></span>|<span data-ttu-id="0b5b6-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="0b5b6-114">Time when the history item occurred.</span></span> <span data-ttu-id="0b5b6-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="0b5b6-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="0b5b6-116">рунстате</span><span class="sxs-lookup"><span data-stu-id="0b5b6-116">runState</span></span>|[<span data-ttu-id="0b5b6-117">рунстате</span><span class="sxs-lookup"><span data-stu-id="0b5b6-117">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="0b5b6-118">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="0b5b6-118">Status of the item.</span></span> <span data-ttu-id="0b5b6-119">Возможные значения: `unknown`, `success`, `fail`, `error`, `pending`.</span><span class="sxs-lookup"><span data-stu-id="0b5b6-119">Possible values are: `unknown`, `success`, `fail`, `error`, `pending`.</span></span>|
|<span data-ttu-id="0b5b6-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="0b5b6-120">errorCode</span></span>|<span data-ttu-id="0b5b6-121">String</span><span class="sxs-lookup"><span data-stu-id="0b5b6-121">String</span></span>|<span data-ttu-id="0b5b6-122">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="0b5b6-122">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b5b6-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="0b5b6-123">Relationships</span></span>
<span data-ttu-id="0b5b6-124">Нет</span><span class="sxs-lookup"><span data-stu-id="0b5b6-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b5b6-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b5b6-125">JSON Representation</span></span>
<span data-ttu-id="0b5b6-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b5b6-126">Here is a JSON representation of the resource.</span></span>
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



