---
title: Тип ресурса microsoftStoreForBusinessAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c42ea0ca8175b22d24061133a8c748f7225e2dd3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755135"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="a098c-103">Тип ресурса microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a098c-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

<span data-ttu-id="a098c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a098c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a098c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a098c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a098c-106">Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.</span><span class="sxs-lookup"><span data-stu-id="a098c-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="a098c-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a098c-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a098c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a098c-108">Properties</span></span>
|<span data-ttu-id="a098c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a098c-109">Property</span></span>|<span data-ttu-id="a098c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a098c-110">Type</span></span>|<span data-ttu-id="a098c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a098c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a098c-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="a098c-112">useDeviceContext</span></span>|<span data-ttu-id="a098c-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="a098c-113">Boolean</span></span>|<span data-ttu-id="a098c-114">Указывает, следует ли использовать контекст работы устройства для мобильного приложения Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a098c-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a098c-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="a098c-115">Relationships</span></span>
<span data-ttu-id="a098c-116">Нет</span><span class="sxs-lookup"><span data-stu-id="a098c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a098c-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a098c-117">JSON Representation</span></span>
<span data-ttu-id="a098c-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a098c-118">Here is a JSON representation of the resource.</span></span>
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




