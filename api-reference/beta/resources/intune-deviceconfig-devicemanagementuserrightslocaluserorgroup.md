---
title: Тип ресурса deviceManagementUserRightsLocalUserOrGroup
description: Представляет сведения для локального пользователя или группы, используемые для настройки прав пользователя.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8a2cc0ff5b9e054398e7878b7d99619b59d109a4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422063"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="5cce7-103">Тип ресурса deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="5cce7-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="5cce7-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5cce7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5cce7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cce7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5cce7-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5cce7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cce7-107">Представляет сведения для локального пользователя или группы, используемые для настройки прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="5cce7-107">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="5cce7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5cce7-108">Properties</span></span>
|<span data-ttu-id="5cce7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cce7-109">Property</span></span>|<span data-ttu-id="5cce7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5cce7-110">Type</span></span>|<span data-ttu-id="5cce7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5cce7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cce7-112">name</span><span class="sxs-lookup"><span data-stu-id="5cce7-112">name</span></span>|<span data-ttu-id="5cce7-113">String</span><span class="sxs-lookup"><span data-stu-id="5cce7-113">String</span></span>|<span data-ttu-id="5cce7-114">Имя этого локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="5cce7-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="5cce7-115">description</span><span class="sxs-lookup"><span data-stu-id="5cce7-115">description</span></span>|<span data-ttu-id="5cce7-116">String</span><span class="sxs-lookup"><span data-stu-id="5cce7-116">String</span></span>|<span data-ttu-id="5cce7-117">Описание администратора локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="5cce7-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="5cce7-118">Класс securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="5cce7-118">securityIdentifier</span></span>|<span data-ttu-id="5cce7-119">String</span><span class="sxs-lookup"><span data-stu-id="5cce7-119">String</span></span>|<span data-ttu-id="5cce7-120">Идентификатор безопасности этого локального пользователя или группы (например \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="5cce7-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cce7-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="5cce7-121">Relationships</span></span>
<span data-ttu-id="5cce7-122">Нет</span><span class="sxs-lookup"><span data-stu-id="5cce7-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cce7-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5cce7-123">JSON Representation</span></span>
<span data-ttu-id="5cce7-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5cce7-124">Here is a JSON representation of the resource.</span></span>
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




