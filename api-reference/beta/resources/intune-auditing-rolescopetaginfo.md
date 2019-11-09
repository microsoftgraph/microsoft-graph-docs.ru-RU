---
title: Тип ресурса Ролескопетагинфо
description: Класс, содержащий свойства объекта тега области применения роли.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 09ddd40d5f24b6c85c3637960a446728830e8dea
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38082769"
---
# <a name="rolescopetaginfo-resource-type"></a><span data-ttu-id="c3575-103">Тип ресурса Ролескопетагинфо</span><span class="sxs-lookup"><span data-stu-id="c3575-103">roleScopeTagInfo resource type</span></span>

> <span data-ttu-id="c3575-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3575-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3575-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3575-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3575-106">Класс, содержащий свойства объекта тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="c3575-106">A class containing the properties of Role Scope Tag Object.</span></span>

## <a name="properties"></a><span data-ttu-id="c3575-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3575-107">Properties</span></span>
|<span data-ttu-id="c3575-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3575-108">Property</span></span>|<span data-ttu-id="c3575-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c3575-109">Type</span></span>|<span data-ttu-id="c3575-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c3575-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3575-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c3575-111">displayName</span></span>|<span data-ttu-id="c3575-112">String</span><span class="sxs-lookup"><span data-stu-id="c3575-112">String</span></span>|<span data-ttu-id="c3575-113">Отображаемое имя тега области.</span><span class="sxs-lookup"><span data-stu-id="c3575-113">Scope Tag Display name.</span></span>|
|<span data-ttu-id="c3575-114">ролескопетагид</span><span class="sxs-lookup"><span data-stu-id="c3575-114">roleScopeTagId</span></span>|<span data-ttu-id="c3575-115">String</span><span class="sxs-lookup"><span data-stu-id="c3575-115">String</span></span>|<span data-ttu-id="c3575-116">Идентификатор тега Scope.</span><span class="sxs-lookup"><span data-stu-id="c3575-116">Scope Tag Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3575-117">Связи</span><span class="sxs-lookup"><span data-stu-id="c3575-117">Relationships</span></span>
<span data-ttu-id="c3575-118">Нет</span><span class="sxs-lookup"><span data-stu-id="c3575-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3575-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3575-119">JSON Representation</span></span>
<span data-ttu-id="c3575-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3575-120">Here is a JSON representation of the resource.</span></span>
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



