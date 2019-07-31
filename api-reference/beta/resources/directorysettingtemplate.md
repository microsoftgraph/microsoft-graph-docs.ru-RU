---
title: Тип ресурса Директорисеттингтемплате
description: Шаблоны параметров каталога представляют системные параметры, доступные для клиента. Параметры каталога могут быть созданы на основе доступных Директорисеттингтемплатес, и значения, заданные по умолчанию, изменяются. Шаблоны параметров каталога невозможно создать, обновить или удалить. Эти параметры могут представлять параметры на уровне клиента или конкретные параметры сущности.  В настоящее время доступны только шаблоны для групп Office, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4239a12be5fffbf5c579752c3de4998c88749bd3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012788"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="8cc15-107">Тип ресурса Директорисеттингтемплате</span><span class="sxs-lookup"><span data-stu-id="8cc15-107">directorySettingTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cc15-108">Шаблоны параметров каталога представляют системные параметры, доступные для клиента.</span><span class="sxs-lookup"><span data-stu-id="8cc15-108">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="8cc15-109">[Параметры каталога](directorysetting.md) могут быть созданы на основе доступных директорисеттингтемплатес, и значения, заданные по умолчанию, изменяются.</span><span class="sxs-lookup"><span data-stu-id="8cc15-109">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="8cc15-110">Шаблоны параметров каталога невозможно создать, обновить или удалить.</span><span class="sxs-lookup"><span data-stu-id="8cc15-110">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="8cc15-111">Эти параметры могут представлять параметры на уровне клиента или конкретные параметры сущности.</span><span class="sxs-lookup"><span data-stu-id="8cc15-111">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="8cc15-112">В настоящее время доступны только шаблоны для групп Office, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.</span><span class="sxs-lookup"><span data-stu-id="8cc15-112">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="8cc15-113">**Note**: версия/Beta типа ресурса директорисеттингтемплате применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="8cc15-113">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="8cc15-114">Версия/v1.0 переименована в groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="8cc15-114">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="8cc15-115">Методы</span><span class="sxs-lookup"><span data-stu-id="8cc15-115">Methods</span></span>

| <span data-ttu-id="8cc15-116">Метод</span><span class="sxs-lookup"><span data-stu-id="8cc15-116">Method</span></span>           | <span data-ttu-id="8cc15-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8cc15-117">Return Type</span></span>    |<span data-ttu-id="8cc15-118">Описание</span><span class="sxs-lookup"><span data-stu-id="8cc15-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8cc15-119">Получение Директорисеттингтемплате</span><span class="sxs-lookup"><span data-stu-id="8cc15-119">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="8cc15-120">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="8cc15-120">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="8cc15-121">Чтение определенных свойств одного из системных объектов Директорисеттингтемплате, определенных системой.</span><span class="sxs-lookup"><span data-stu-id="8cc15-121">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="8cc15-122">Список Директорисеттингтемплате</span><span class="sxs-lookup"><span data-stu-id="8cc15-122">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="8cc15-123">Коллекция Директорисеттингтемплате</span><span class="sxs-lookup"><span data-stu-id="8cc15-123">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="8cc15-124">Перечисление всех объектов Директорисеттингтемплате, определенных системой.</span><span class="sxs-lookup"><span data-stu-id="8cc15-124">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="8cc15-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="8cc15-125">Properties</span></span>
| <span data-ttu-id="8cc15-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cc15-126">Property</span></span>     | <span data-ttu-id="8cc15-127">Тип</span><span class="sxs-lookup"><span data-stu-id="8cc15-127">Type</span></span>   |<span data-ttu-id="8cc15-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8cc15-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cc15-129">description</span><span class="sxs-lookup"><span data-stu-id="8cc15-129">description</span></span>|<span data-ttu-id="8cc15-130">string</span><span class="sxs-lookup"><span data-stu-id="8cc15-130">string</span></span>|<span data-ttu-id="8cc15-131">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="8cc15-131">Description of the template.</span></span> <span data-ttu-id="8cc15-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8cc15-132">Read-only.</span></span>|
|<span data-ttu-id="8cc15-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8cc15-133">displayName</span></span>|<span data-ttu-id="8cc15-134">string</span><span class="sxs-lookup"><span data-stu-id="8cc15-134">string</span></span>|<span data-ttu-id="8cc15-135">Отображаемое имя шаблона.</span><span class="sxs-lookup"><span data-stu-id="8cc15-135">Display name of the template.</span></span> <span data-ttu-id="8cc15-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8cc15-136">Read-only.</span></span> |
|<span data-ttu-id="8cc15-137">id</span><span class="sxs-lookup"><span data-stu-id="8cc15-137">id</span></span>|<span data-ttu-id="8cc15-138">string</span><span class="sxs-lookup"><span data-stu-id="8cc15-138">string</span></span>| <span data-ttu-id="8cc15-139">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="8cc15-139">Unique identifier for the template.</span></span> <span data-ttu-id="8cc15-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8cc15-140">Read-only.</span></span>|
|<span data-ttu-id="8cc15-141">values</span><span class="sxs-lookup"><span data-stu-id="8cc15-141">values</span></span>|<span data-ttu-id="8cc15-142">Коллекция [сеттингтемплатевалуе](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="8cc15-142">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="8cc15-143">Коллекция Settingtemplatevalue, в которой перечислены набор доступных параметров, значения по умолчанию и типы, которые составляют этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="8cc15-143">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="8cc15-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8cc15-144">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8cc15-145">Отношения</span><span class="sxs-lookup"><span data-stu-id="8cc15-145">Relationships</span></span>
<span data-ttu-id="8cc15-146">Нет</span><span class="sxs-lookup"><span data-stu-id="8cc15-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8cc15-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8cc15-147">JSON representation</span></span>

<span data-ttu-id="8cc15-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8cc15-148">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySettingTemplate"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
