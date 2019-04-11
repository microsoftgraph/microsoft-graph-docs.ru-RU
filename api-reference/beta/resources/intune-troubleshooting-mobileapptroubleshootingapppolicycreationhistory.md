---
title: Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори
description: Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbbf575c7eaecb93e0256d6f672d0c4d6bdd0edf
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802494"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="0d31a-103">Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори</span><span class="sxs-lookup"><span data-stu-id="0d31a-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="0d31a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d31a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d31a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d31a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d31a-106">Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="0d31a-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="0d31a-107">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="0d31a-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0d31a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d31a-108">Properties</span></span>
|<span data-ttu-id="0d31a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d31a-109">Property</span></span>|<span data-ttu-id="0d31a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0d31a-110">Type</span></span>|<span data-ttu-id="0d31a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0d31a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d31a-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="0d31a-112">occurrenceDateTime</span></span>|<span data-ttu-id="0d31a-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d31a-113">DateTimeOffset</span></span>|<span data-ttu-id="0d31a-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="0d31a-114">Time when the history item occurred.</span></span> <span data-ttu-id="0d31a-115">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="0d31a-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="0d31a-116">Рунстате</span><span class="sxs-lookup"><span data-stu-id="0d31a-116">runState</span></span>|[<span data-ttu-id="0d31a-117">Рунстате</span><span class="sxs-lookup"><span data-stu-id="0d31a-117">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="0d31a-118">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="0d31a-118">Status of the item.</span></span> <span data-ttu-id="0d31a-119">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="0d31a-119">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="0d31a-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="0d31a-120">errorCode</span></span>|<span data-ttu-id="0d31a-121">String</span><span class="sxs-lookup"><span data-stu-id="0d31a-121">String</span></span>|<span data-ttu-id="0d31a-122">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="0d31a-122">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d31a-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="0d31a-123">Relationships</span></span>
<span data-ttu-id="0d31a-124">Нет</span><span class="sxs-lookup"><span data-stu-id="0d31a-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d31a-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d31a-125">JSON Representation</span></span>
<span data-ttu-id="0d31a-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d31a-126">Here is a JSON representation of the resource.</span></span>
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



