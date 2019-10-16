---
title: Тип ресурса Скопетагинфо
description: Класс, содержащий свойства объекта тега области.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8238881d8a14cb8aa1dfcc01031105be0069c21
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538506"
---
# <a name="scopetaginfo-resource-type"></a><span data-ttu-id="c23a7-103">Тип ресурса Скопетагинфо</span><span class="sxs-lookup"><span data-stu-id="c23a7-103">scopeTagInfo resource type</span></span>

> <span data-ttu-id="c23a7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c23a7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c23a7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c23a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c23a7-106">Класс, содержащий свойства объекта тега области.</span><span class="sxs-lookup"><span data-stu-id="c23a7-106">A class containing the properties of Scope Tag Object.</span></span>

## <a name="properties"></a><span data-ttu-id="c23a7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c23a7-107">Properties</span></span>
|<span data-ttu-id="c23a7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c23a7-108">Property</span></span>|<span data-ttu-id="c23a7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c23a7-109">Type</span></span>|<span data-ttu-id="c23a7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c23a7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c23a7-111">скопетагнаме</span><span class="sxs-lookup"><span data-stu-id="c23a7-111">scopeTagName</span></span>|<span data-ttu-id="c23a7-112">String</span><span class="sxs-lookup"><span data-stu-id="c23a7-112">String</span></span>|<span data-ttu-id="c23a7-113">Отображаемое имя тега области.</span><span class="sxs-lookup"><span data-stu-id="c23a7-113">Scope Tag Display name.</span></span>|
|<span data-ttu-id="c23a7-114">скопетагид</span><span class="sxs-lookup"><span data-stu-id="c23a7-114">scopeTagId</span></span>|<span data-ttu-id="c23a7-115">String</span><span class="sxs-lookup"><span data-stu-id="c23a7-115">String</span></span>|<span data-ttu-id="c23a7-116">Идентификатор тега Scope.</span><span class="sxs-lookup"><span data-stu-id="c23a7-116">Scope Tag Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c23a7-117">Связи</span><span class="sxs-lookup"><span data-stu-id="c23a7-117">Relationships</span></span>
<span data-ttu-id="c23a7-118">Нет</span><span class="sxs-lookup"><span data-stu-id="c23a7-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c23a7-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c23a7-119">JSON Representation</span></span>
<span data-ttu-id="c23a7-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c23a7-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.scopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.scopeTagInfo",
  "scopeTagName": "String",
  "scopeTagId": "String"
}
```



