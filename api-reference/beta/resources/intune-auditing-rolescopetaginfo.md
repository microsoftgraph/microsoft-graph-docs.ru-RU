---
title: Тип ресурса Ролескопетагинфо
description: Класс, содержащий свойства объекта тега области применения роли.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c932a1353f684771a1979ae970141d674f726142
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797411"
---
# <a name="rolescopetaginfo-resource-type"></a><span data-ttu-id="a32a5-103">Тип ресурса Ролескопетагинфо</span><span class="sxs-lookup"><span data-stu-id="a32a5-103">roleScopeTagInfo resource type</span></span>

> <span data-ttu-id="a32a5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a32a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a32a5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a32a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a32a5-106">Класс, содержащий свойства объекта тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="a32a5-106">A class containing the properties of Role Scope Tag Object.</span></span>

## <a name="properties"></a><span data-ttu-id="a32a5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a32a5-107">Properties</span></span>
|<span data-ttu-id="a32a5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a32a5-108">Property</span></span>|<span data-ttu-id="a32a5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a32a5-109">Type</span></span>|<span data-ttu-id="a32a5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a32a5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a32a5-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a32a5-111">displayName</span></span>|<span data-ttu-id="a32a5-112">String</span><span class="sxs-lookup"><span data-stu-id="a32a5-112">String</span></span>|<span data-ttu-id="a32a5-113">Отображаемое имя тега области.</span><span class="sxs-lookup"><span data-stu-id="a32a5-113">Scope Tag Display name.</span></span>|
|<span data-ttu-id="a32a5-114">ролескопетагид</span><span class="sxs-lookup"><span data-stu-id="a32a5-114">roleScopeTagId</span></span>|<span data-ttu-id="a32a5-115">String</span><span class="sxs-lookup"><span data-stu-id="a32a5-115">String</span></span>|<span data-ttu-id="a32a5-116">Идентификатор тега Scope.</span><span class="sxs-lookup"><span data-stu-id="a32a5-116">Scope Tag Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a32a5-117">Связи</span><span class="sxs-lookup"><span data-stu-id="a32a5-117">Relationships</span></span>
<span data-ttu-id="a32a5-118">Нет</span><span class="sxs-lookup"><span data-stu-id="a32a5-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a32a5-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a32a5-119">JSON Representation</span></span>
<span data-ttu-id="a32a5-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a32a5-120">Here is a JSON representation of the resource.</span></span>
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



