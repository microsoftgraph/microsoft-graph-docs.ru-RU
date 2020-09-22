---
title: Тип ресурса microsoftStoreForBusinessAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 32186cd4c5b4321d668e350b5f03ec6e127399cd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094458"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="fc24c-103">Тип ресурса microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="fc24c-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

<span data-ttu-id="fc24c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc24c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc24c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc24c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc24c-106">Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.</span><span class="sxs-lookup"><span data-stu-id="fc24c-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="fc24c-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="fc24c-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fc24c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc24c-108">Properties</span></span>
|<span data-ttu-id="fc24c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc24c-109">Property</span></span>|<span data-ttu-id="fc24c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fc24c-110">Type</span></span>|<span data-ttu-id="fc24c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fc24c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc24c-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="fc24c-112">useDeviceContext</span></span>|<span data-ttu-id="fc24c-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc24c-113">Boolean</span></span>|<span data-ttu-id="fc24c-114">Указывает, следует ли использовать контекст работы устройства для мобильного приложения Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="fc24c-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc24c-115">Связи</span><span class="sxs-lookup"><span data-stu-id="fc24c-115">Relationships</span></span>
<span data-ttu-id="fc24c-116">Нет</span><span class="sxs-lookup"><span data-stu-id="fc24c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc24c-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc24c-117">JSON Representation</span></span>
<span data-ttu-id="fc24c-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc24c-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```









