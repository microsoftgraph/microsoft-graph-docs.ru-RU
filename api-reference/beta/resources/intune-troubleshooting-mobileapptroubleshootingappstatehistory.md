---
title: Тип ресурса Мобилеапптраублешутингаппстатехистори
description: Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75285b5dec8b3b3808f2e81a4655d9298d12d486
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570668"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="b2f1d-103">Тип ресурса Мобилеапптраублешутингаппстатехистори</span><span class="sxs-lookup"><span data-stu-id="b2f1d-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="b2f1d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2f1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2f1d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2f1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2f1d-106">Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="b2f1d-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="b2f1d-107">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b2f1d-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b2f1d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2f1d-108">Properties</span></span>
|<span data-ttu-id="b2f1d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2f1d-109">Property</span></span>|<span data-ttu-id="b2f1d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b2f1d-110">Type</span></span>|<span data-ttu-id="b2f1d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b2f1d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2f1d-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="b2f1d-112">occurrenceDateTime</span></span>|<span data-ttu-id="b2f1d-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2f1d-113">DateTimeOffset</span></span>|<span data-ttu-id="b2f1d-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="b2f1d-114">Time when the history item occurred.</span></span> <span data-ttu-id="b2f1d-115">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b2f1d-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="b2f1d-116">actionType</span><span class="sxs-lookup"><span data-stu-id="b2f1d-116">actionType</span></span>|<span data-ttu-id="b2f1d-117">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md);</span><span class="sxs-lookup"><span data-stu-id="b2f1d-117">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md)</span></span>|<span data-ttu-id="b2f1d-118">Идентификатор группы безопасности AAD, к которой назначена эта группа.</span><span class="sxs-lookup"><span data-stu-id="b2f1d-118">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="b2f1d-119">Возможные значения: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="b2f1d-119">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="b2f1d-120">Рунстате</span><span class="sxs-lookup"><span data-stu-id="b2f1d-120">runState</span></span>|[<span data-ttu-id="b2f1d-121">Рунстате</span><span class="sxs-lookup"><span data-stu-id="b2f1d-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="b2f1d-122">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="b2f1d-122">Status of the item.</span></span> <span data-ttu-id="b2f1d-123">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="b2f1d-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="b2f1d-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="b2f1d-124">errorCode</span></span>|<span data-ttu-id="b2f1d-125">String</span><span class="sxs-lookup"><span data-stu-id="b2f1d-125">String</span></span>|<span data-ttu-id="b2f1d-126">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="b2f1d-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2f1d-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="b2f1d-127">Relationships</span></span>
<span data-ttu-id="b2f1d-128">Нет</span><span class="sxs-lookup"><span data-stu-id="b2f1d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2f1d-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2f1d-129">JSON Representation</span></span>
<span data-ttu-id="b2f1d-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2f1d-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppStateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppStateHistory",
  "occurrenceDateTime": "String (timestamp)",
  "actionType": "String",
  "runState": "String",
  "errorCode": "String"
}
```



