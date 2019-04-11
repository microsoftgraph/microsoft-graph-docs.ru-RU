---
title: Тип ресурса Мобилеапптраублешутингапптаржесистори
description: Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a19399788462b6dc7cae995971ddb443051b6959
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774654"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="5e56a-103">Тип ресурса Мобилеапптраублешутингапптаржесистори</span><span class="sxs-lookup"><span data-stu-id="5e56a-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="5e56a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e56a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e56a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e56a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e56a-106">Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="5e56a-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="5e56a-107">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5e56a-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5e56a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e56a-108">Properties</span></span>
|<span data-ttu-id="5e56a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e56a-109">Property</span></span>|<span data-ttu-id="5e56a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5e56a-110">Type</span></span>|<span data-ttu-id="5e56a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5e56a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e56a-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="5e56a-112">occurrenceDateTime</span></span>|<span data-ttu-id="5e56a-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e56a-113">DateTimeOffset</span></span>|<span data-ttu-id="5e56a-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="5e56a-114">Time when the history item occurred.</span></span> <span data-ttu-id="5e56a-115">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5e56a-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="5e56a-116">Секуритиграупид</span><span class="sxs-lookup"><span data-stu-id="5e56a-116">securityGroupId</span></span>|<span data-ttu-id="5e56a-117">String</span><span class="sxs-lookup"><span data-stu-id="5e56a-117">String</span></span>|<span data-ttu-id="5e56a-118">Идентификатор группы безопасности AAD, к которой назначена эта группа.</span><span class="sxs-lookup"><span data-stu-id="5e56a-118">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="5e56a-119">Рунстате</span><span class="sxs-lookup"><span data-stu-id="5e56a-119">runState</span></span>|[<span data-ttu-id="5e56a-120">Рунстате</span><span class="sxs-lookup"><span data-stu-id="5e56a-120">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="5e56a-121">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="5e56a-121">Status of the item.</span></span> <span data-ttu-id="5e56a-122">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="5e56a-122">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="5e56a-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="5e56a-123">errorCode</span></span>|<span data-ttu-id="5e56a-124">String</span><span class="sxs-lookup"><span data-stu-id="5e56a-124">String</span></span>|<span data-ttu-id="5e56a-125">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="5e56a-125">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e56a-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="5e56a-126">Relationships</span></span>
<span data-ttu-id="5e56a-127">Нет</span><span class="sxs-lookup"><span data-stu-id="5e56a-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e56a-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e56a-128">JSON Representation</span></span>
<span data-ttu-id="5e56a-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e56a-129">Here is a JSON representation of the resource.</span></span>
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



