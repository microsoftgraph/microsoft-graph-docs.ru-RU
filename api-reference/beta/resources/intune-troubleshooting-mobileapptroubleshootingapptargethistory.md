---
title: Тип ресурса Мобилеапптраублешутингапптаржесистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3964702646476f35f7f6e9b7928b69fca83dc5e8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371308"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="4bb13-103">Тип ресурса Мобилеапптраублешутингапптаржесистори</span><span class="sxs-lookup"><span data-stu-id="4bb13-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="4bb13-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bb13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bb13-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4bb13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bb13-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="4bb13-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="4bb13-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="4bb13-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4bb13-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4bb13-108">Properties</span></span>
|<span data-ttu-id="4bb13-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bb13-109">Property</span></span>|<span data-ttu-id="4bb13-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4bb13-110">Type</span></span>|<span data-ttu-id="4bb13-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4bb13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bb13-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="4bb13-112">occurrenceDateTime</span></span>|<span data-ttu-id="4bb13-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bb13-113">DateTimeOffset</span></span>|<span data-ttu-id="4bb13-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="4bb13-114">Time when the history item occurred.</span></span> <span data-ttu-id="4bb13-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="4bb13-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="4bb13-116">секуритиграупид</span><span class="sxs-lookup"><span data-stu-id="4bb13-116">securityGroupId</span></span>|<span data-ttu-id="4bb13-117">String</span><span class="sxs-lookup"><span data-stu-id="4bb13-117">String</span></span>|<span data-ttu-id="4bb13-118">Идентификатор группы безопасности AAD, к которой назначена эта группа.</span><span class="sxs-lookup"><span data-stu-id="4bb13-118">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="4bb13-119">рунстате</span><span class="sxs-lookup"><span data-stu-id="4bb13-119">runState</span></span>|[<span data-ttu-id="4bb13-120">рунстате</span><span class="sxs-lookup"><span data-stu-id="4bb13-120">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="4bb13-121">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="4bb13-121">Status of the item.</span></span> <span data-ttu-id="4bb13-122">Возможные значения: `unknown`, `success`, `fail`, `error`, `pending`.</span><span class="sxs-lookup"><span data-stu-id="4bb13-122">Possible values are: `unknown`, `success`, `fail`, `error`, `pending`.</span></span>|
|<span data-ttu-id="4bb13-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="4bb13-123">errorCode</span></span>|<span data-ttu-id="4bb13-124">String</span><span class="sxs-lookup"><span data-stu-id="4bb13-124">String</span></span>|<span data-ttu-id="4bb13-125">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="4bb13-125">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4bb13-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="4bb13-126">Relationships</span></span>
<span data-ttu-id="4bb13-127">Нет</span><span class="sxs-lookup"><span data-stu-id="4bb13-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4bb13-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4bb13-128">JSON Representation</span></span>
<span data-ttu-id="4bb13-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4bb13-129">Here is a JSON representation of the resource.</span></span>
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



