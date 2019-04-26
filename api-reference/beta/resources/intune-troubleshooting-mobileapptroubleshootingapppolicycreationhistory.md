---
title: Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори
description: Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbbf575c7eaecb93e0256d6f672d0c4d6bdd0edf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570042"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="68288-103">Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори</span><span class="sxs-lookup"><span data-stu-id="68288-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="68288-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68288-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68288-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68288-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68288-106">Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="68288-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="68288-107">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="68288-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="68288-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="68288-108">Properties</span></span>
|<span data-ttu-id="68288-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="68288-109">Property</span></span>|<span data-ttu-id="68288-110">Тип</span><span class="sxs-lookup"><span data-stu-id="68288-110">Type</span></span>|<span data-ttu-id="68288-111">Описание</span><span class="sxs-lookup"><span data-stu-id="68288-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68288-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="68288-112">occurrenceDateTime</span></span>|<span data-ttu-id="68288-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68288-113">DateTimeOffset</span></span>|<span data-ttu-id="68288-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="68288-114">Time when the history item occurred.</span></span> <span data-ttu-id="68288-115">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="68288-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="68288-116">Рунстате</span><span class="sxs-lookup"><span data-stu-id="68288-116">runState</span></span>|[<span data-ttu-id="68288-117">Рунстате</span><span class="sxs-lookup"><span data-stu-id="68288-117">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="68288-118">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="68288-118">Status of the item.</span></span> <span data-ttu-id="68288-119">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="68288-119">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="68288-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="68288-120">errorCode</span></span>|<span data-ttu-id="68288-121">String</span><span class="sxs-lookup"><span data-stu-id="68288-121">String</span></span>|<span data-ttu-id="68288-122">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="68288-122">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68288-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="68288-123">Relationships</span></span>
<span data-ttu-id="68288-124">Нет</span><span class="sxs-lookup"><span data-stu-id="68288-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68288-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68288-125">JSON Representation</span></span>
<span data-ttu-id="68288-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68288-126">Here is a JSON representation of the resource.</span></span>
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



