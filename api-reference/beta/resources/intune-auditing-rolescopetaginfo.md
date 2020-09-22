---
title: Тип ресурса Ролескопетагинфо
description: Класс, содержащий свойства объекта тега области применения роли.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67927894be0f4209e915781169a45d5daa874b20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076246"
---
# <a name="rolescopetaginfo-resource-type"></a><span data-ttu-id="67d0d-103">Тип ресурса Ролескопетагинфо</span><span class="sxs-lookup"><span data-stu-id="67d0d-103">roleScopeTagInfo resource type</span></span>

<span data-ttu-id="67d0d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67d0d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67d0d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67d0d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67d0d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="67d0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67d0d-107">Класс, содержащий свойства объекта тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="67d0d-107">A class containing the properties of Role Scope Tag Object.</span></span>

## <a name="properties"></a><span data-ttu-id="67d0d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="67d0d-108">Properties</span></span>
|<span data-ttu-id="67d0d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="67d0d-109">Property</span></span>|<span data-ttu-id="67d0d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="67d0d-110">Type</span></span>|<span data-ttu-id="67d0d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="67d0d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67d0d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="67d0d-112">displayName</span></span>|<span data-ttu-id="67d0d-113">String</span><span class="sxs-lookup"><span data-stu-id="67d0d-113">String</span></span>|<span data-ttu-id="67d0d-114">Отображаемое имя тега области.</span><span class="sxs-lookup"><span data-stu-id="67d0d-114">Scope Tag Display name.</span></span>|
|<span data-ttu-id="67d0d-115">ролескопетагид</span><span class="sxs-lookup"><span data-stu-id="67d0d-115">roleScopeTagId</span></span>|<span data-ttu-id="67d0d-116">String</span><span class="sxs-lookup"><span data-stu-id="67d0d-116">String</span></span>|<span data-ttu-id="67d0d-117">Идентификатор тега Scope.</span><span class="sxs-lookup"><span data-stu-id="67d0d-117">Scope Tag Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67d0d-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="67d0d-118">Relationships</span></span>
<span data-ttu-id="67d0d-119">Нет</span><span class="sxs-lookup"><span data-stu-id="67d0d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67d0d-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67d0d-120">JSON Representation</span></span>
<span data-ttu-id="67d0d-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67d0d-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.roleScopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagInfo",
  "displayName": "String",
  "roleScopeTagId": "String"
}
```






