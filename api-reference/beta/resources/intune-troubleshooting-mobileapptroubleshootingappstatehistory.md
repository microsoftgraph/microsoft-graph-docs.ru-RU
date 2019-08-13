---
title: Тип ресурса Мобилеапптраублешутингаппстатехистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 62c57d4ed01ab1f454a5356899f9645927680dfd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313050"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="6fcbe-103">Тип ресурса Мобилеапптраублешутингаппстатехистори</span><span class="sxs-lookup"><span data-stu-id="6fcbe-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="6fcbe-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fcbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fcbe-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6fcbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fcbe-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="6fcbe-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="6fcbe-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="6fcbe-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6fcbe-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6fcbe-108">Properties</span></span>
|<span data-ttu-id="6fcbe-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fcbe-109">Property</span></span>|<span data-ttu-id="6fcbe-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6fcbe-110">Type</span></span>|<span data-ttu-id="6fcbe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6fcbe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fcbe-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="6fcbe-112">occurrenceDateTime</span></span>|<span data-ttu-id="6fcbe-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fcbe-113">DateTimeOffset</span></span>|<span data-ttu-id="6fcbe-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="6fcbe-114">Time when the history item occurred.</span></span> <span data-ttu-id="6fcbe-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="6fcbe-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="6fcbe-116">actionType</span><span class="sxs-lookup"><span data-stu-id="6fcbe-116">actionType</span></span>|<span data-ttu-id="6fcbe-117">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md);</span><span class="sxs-lookup"><span data-stu-id="6fcbe-117">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md)</span></span>|<span data-ttu-id="6fcbe-118">Идентификатор группы безопасности AAD, к которой назначена эта группа.</span><span class="sxs-lookup"><span data-stu-id="6fcbe-118">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="6fcbe-119">Возможные значения: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="6fcbe-119">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="6fcbe-120">рунстате</span><span class="sxs-lookup"><span data-stu-id="6fcbe-120">runState</span></span>|[<span data-ttu-id="6fcbe-121">рунстате</span><span class="sxs-lookup"><span data-stu-id="6fcbe-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="6fcbe-122">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="6fcbe-122">Status of the item.</span></span> <span data-ttu-id="6fcbe-123">Возможные значения: `unknown`, `success`, `fail`, `error`, `pending`.</span><span class="sxs-lookup"><span data-stu-id="6fcbe-123">Possible values are: `unknown`, `success`, `fail`, `error`, `pending`.</span></span>|
|<span data-ttu-id="6fcbe-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="6fcbe-124">errorCode</span></span>|<span data-ttu-id="6fcbe-125">String</span><span class="sxs-lookup"><span data-stu-id="6fcbe-125">String</span></span>|<span data-ttu-id="6fcbe-126">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="6fcbe-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fcbe-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="6fcbe-127">Relationships</span></span>
<span data-ttu-id="6fcbe-128">Нет</span><span class="sxs-lookup"><span data-stu-id="6fcbe-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fcbe-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6fcbe-129">JSON Representation</span></span>
<span data-ttu-id="6fcbe-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fcbe-130">Here is a JSON representation of the resource.</span></span>
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



