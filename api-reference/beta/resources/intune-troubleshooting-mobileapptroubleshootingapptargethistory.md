---
title: Тип ресурса Мобилеапптраублешутингапптаржесистори
description: Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a7171cdde4889ba97a9cd29c4cc8c81ab1a9d58
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159355"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="4b531-103">Тип ресурса Мобилеапптраублешутингапптаржесистори</span><span class="sxs-lookup"><span data-stu-id="4b531-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="4b531-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b531-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b531-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b531-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b531-106">Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="4b531-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="4b531-107">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="4b531-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4b531-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b531-108">Properties</span></span>
|<span data-ttu-id="4b531-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b531-109">Property</span></span>|<span data-ttu-id="4b531-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4b531-110">Type</span></span>|<span data-ttu-id="4b531-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4b531-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b531-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="4b531-112">occurrenceDateTime</span></span>|<span data-ttu-id="4b531-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b531-113">DateTimeOffset</span></span>|<span data-ttu-id="4b531-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="4b531-114">Time when the history item occurred.</span></span> <span data-ttu-id="4b531-115">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="4b531-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="4b531-116">Секуритиграупид</span><span class="sxs-lookup"><span data-stu-id="4b531-116">securityGroupId</span></span>|<span data-ttu-id="4b531-117">String</span><span class="sxs-lookup"><span data-stu-id="4b531-117">String</span></span>|<span data-ttu-id="4b531-118">Идентификатор группы безопасности AAD, к которой назначена эта группа.</span><span class="sxs-lookup"><span data-stu-id="4b531-118">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="4b531-119">Рунстате</span><span class="sxs-lookup"><span data-stu-id="4b531-119">runState</span></span>|[<span data-ttu-id="4b531-120">Рунстате</span><span class="sxs-lookup"><span data-stu-id="4b531-120">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="4b531-121">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="4b531-121">Status of the item.</span></span> <span data-ttu-id="4b531-122">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="4b531-122">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="4b531-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="4b531-123">errorCode</span></span>|<span data-ttu-id="4b531-124">String</span><span class="sxs-lookup"><span data-stu-id="4b531-124">String</span></span>|<span data-ttu-id="4b531-125">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="4b531-125">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b531-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="4b531-126">Relationships</span></span>
<span data-ttu-id="4b531-127">Нет</span><span class="sxs-lookup"><span data-stu-id="4b531-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b531-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b531-128">JSON Representation</span></span>
<span data-ttu-id="4b531-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b531-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppTargetHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppTargetHistory",
  "occurrenceDateTime": "String (timestamp)",
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```




