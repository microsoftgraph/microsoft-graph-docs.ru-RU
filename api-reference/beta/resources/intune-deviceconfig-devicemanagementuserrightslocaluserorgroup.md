---
title: Тип ресурса Девицеманажементусерригхтслокалусерорграуп
description: Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a4e935781bf0524f5fb5df2a8a9ecd868767bfed
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530120"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="d4b90-103">Тип ресурса Девицеманажементусерригхтслокалусерорграуп</span><span class="sxs-lookup"><span data-stu-id="d4b90-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

<span data-ttu-id="d4b90-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d4b90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4b90-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4b90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4b90-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4b90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4b90-107">Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="d4b90-107">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="d4b90-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4b90-108">Properties</span></span>
|<span data-ttu-id="d4b90-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4b90-109">Property</span></span>|<span data-ttu-id="d4b90-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d4b90-110">Type</span></span>|<span data-ttu-id="d4b90-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d4b90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4b90-112">name</span><span class="sxs-lookup"><span data-stu-id="d4b90-112">name</span></span>|<span data-ttu-id="d4b90-113">String</span><span class="sxs-lookup"><span data-stu-id="d4b90-113">String</span></span>|<span data-ttu-id="d4b90-114">Имя локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="d4b90-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="d4b90-115">description</span><span class="sxs-lookup"><span data-stu-id="d4b90-115">description</span></span>|<span data-ttu-id="d4b90-116">String</span><span class="sxs-lookup"><span data-stu-id="d4b90-116">String</span></span>|<span data-ttu-id="d4b90-117">Описание локального пользователя или группы администратором.</span><span class="sxs-lookup"><span data-stu-id="d4b90-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="d4b90-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="d4b90-118">securityIdentifier</span></span>|<span data-ttu-id="d4b90-119">String</span><span class="sxs-lookup"><span data-stu-id="d4b90-119">String</span></span>|<span data-ttu-id="d4b90-120">Идентификатор безопасности этого локального пользователя или группы (например, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="d4b90-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4b90-121">Связи</span><span class="sxs-lookup"><span data-stu-id="d4b90-121">Relationships</span></span>
<span data-ttu-id="d4b90-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d4b90-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4b90-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4b90-123">JSON Representation</span></span>
<span data-ttu-id="d4b90-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4b90-124">Here is a JSON representation of the resource.</span></span>
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



