---
title: Тип ресурса deviceManagementUserRightsLocalUserOrGroup
description: Представляет сведения для локального пользователя или группы, используемые для настройки прав пользователя.
ms.openlocfilehash: bf81a36a8e102bea4c3e8fb56e45bf7822cf31a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078975"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="d1f68-103">Тип ресурса deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="d1f68-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="d1f68-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d1f68-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1f68-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1f68-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1f68-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d1f68-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1f68-107">Представляет сведения для локального пользователя или группы, используемые для настройки прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="d1f68-107">Represents information for a local user or group used for user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="d1f68-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1f68-108">Properties</span></span>
|<span data-ttu-id="d1f68-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1f68-109">Property</span></span>|<span data-ttu-id="d1f68-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d1f68-110">Type</span></span>|<span data-ttu-id="d1f68-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d1f68-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1f68-112">name</span><span class="sxs-lookup"><span data-stu-id="d1f68-112">name</span></span>|<span data-ttu-id="d1f68-113">String</span><span class="sxs-lookup"><span data-stu-id="d1f68-113">String</span></span>|<span data-ttu-id="d1f68-114">Имя этого локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="d1f68-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="d1f68-115">описание</span><span class="sxs-lookup"><span data-stu-id="d1f68-115">description</span></span>|<span data-ttu-id="d1f68-116">String</span><span class="sxs-lookup"><span data-stu-id="d1f68-116">String</span></span>|<span data-ttu-id="d1f68-117">Описание администратора локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="d1f68-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="d1f68-118">Класс securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="d1f68-118">securityIdentifier</span></span>|<span data-ttu-id="d1f68-119">String</span><span class="sxs-lookup"><span data-stu-id="d1f68-119">String</span></span>|<span data-ttu-id="d1f68-120">Идентификатор безопасности этого локального пользователя или группы (например \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="d1f68-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1f68-121">Связи</span><span class="sxs-lookup"><span data-stu-id="d1f68-121">Relationships</span></span>
<span data-ttu-id="d1f68-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d1f68-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d1f68-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1f68-123">JSON Representation</span></span>
<span data-ttu-id="d1f68-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1f68-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```





