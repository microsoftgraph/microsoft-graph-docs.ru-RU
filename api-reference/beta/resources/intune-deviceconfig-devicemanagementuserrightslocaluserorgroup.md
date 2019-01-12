---
title: Тип ресурса deviceManagementUserRightsLocalUserOrGroup
description: Представляет сведения для локального пользователя или группы, используемые для настройки прав пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 63e2dc3d16d17b76c4437e76eae642976711071c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972896"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="4d29e-103">Тип ресурса deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="4d29e-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="4d29e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4d29e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d29e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d29e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d29e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4d29e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d29e-107">Представляет сведения для локального пользователя или группы, используемые для настройки прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="4d29e-107">Represents information for a local user or group used for user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="4d29e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d29e-108">Properties</span></span>
|<span data-ttu-id="4d29e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d29e-109">Property</span></span>|<span data-ttu-id="4d29e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4d29e-110">Type</span></span>|<span data-ttu-id="4d29e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4d29e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d29e-112">name</span><span class="sxs-lookup"><span data-stu-id="4d29e-112">name</span></span>|<span data-ttu-id="4d29e-113">Строка</span><span class="sxs-lookup"><span data-stu-id="4d29e-113">String</span></span>|<span data-ttu-id="4d29e-114">Имя этого локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="4d29e-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="4d29e-115">описание</span><span class="sxs-lookup"><span data-stu-id="4d29e-115">description</span></span>|<span data-ttu-id="4d29e-116">Строка</span><span class="sxs-lookup"><span data-stu-id="4d29e-116">String</span></span>|<span data-ttu-id="4d29e-117">Описание администратора локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="4d29e-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="4d29e-118">Класс securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="4d29e-118">securityIdentifier</span></span>|<span data-ttu-id="4d29e-119">Строка</span><span class="sxs-lookup"><span data-stu-id="4d29e-119">String</span></span>|<span data-ttu-id="4d29e-120">Идентификатор безопасности этого локального пользователя или группы (например \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="4d29e-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d29e-121">Связи</span><span class="sxs-lookup"><span data-stu-id="4d29e-121">Relationships</span></span>
<span data-ttu-id="4d29e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="4d29e-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4d29e-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d29e-123">JSON Representation</span></span>
<span data-ttu-id="4d29e-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d29e-124">Here is a JSON representation of the resource.</span></span>
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





