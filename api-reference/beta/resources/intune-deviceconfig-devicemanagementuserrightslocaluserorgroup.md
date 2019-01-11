---
title: Тип ресурса deviceManagementUserRightsLocalUserOrGroup
description: Представляет сведения для локального пользователя или группы, используемые для настройки прав пользователя.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d795e2b259c71612b1d0720796b6ad76145bb36d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885745"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="3a498-103">Тип ресурса deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="3a498-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="3a498-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3a498-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a498-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a498-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a498-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3a498-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a498-107">Представляет сведения для локального пользователя или группы, используемые для настройки прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="3a498-107">Represents information for a local user or group used for user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="3a498-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a498-108">Properties</span></span>
|<span data-ttu-id="3a498-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a498-109">Property</span></span>|<span data-ttu-id="3a498-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3a498-110">Type</span></span>|<span data-ttu-id="3a498-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3a498-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a498-112">name</span><span class="sxs-lookup"><span data-stu-id="3a498-112">name</span></span>|<span data-ttu-id="3a498-113">Строка</span><span class="sxs-lookup"><span data-stu-id="3a498-113">String</span></span>|<span data-ttu-id="3a498-114">Имя этого локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="3a498-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="3a498-115">описание</span><span class="sxs-lookup"><span data-stu-id="3a498-115">description</span></span>|<span data-ttu-id="3a498-116">Строка</span><span class="sxs-lookup"><span data-stu-id="3a498-116">String</span></span>|<span data-ttu-id="3a498-117">Описание администратора локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="3a498-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="3a498-118">Класс securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="3a498-118">securityIdentifier</span></span>|<span data-ttu-id="3a498-119">Строка</span><span class="sxs-lookup"><span data-stu-id="3a498-119">String</span></span>|<span data-ttu-id="3a498-120">Идентификатор безопасности этого локального пользователя или группы (например \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="3a498-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a498-121">Связи</span><span class="sxs-lookup"><span data-stu-id="3a498-121">Relationships</span></span>
<span data-ttu-id="3a498-122">Нет</span><span class="sxs-lookup"><span data-stu-id="3a498-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3a498-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3a498-123">JSON Representation</span></span>
<span data-ttu-id="3a498-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a498-124">Here is a JSON representation of the resource.</span></span>
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





