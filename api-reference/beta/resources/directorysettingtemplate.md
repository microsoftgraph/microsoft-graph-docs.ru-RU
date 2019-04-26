---
title: Тип ресурса Директорисеттингтемплате
description: Шаблоны параметров каталога представляют системные параметры, доступные для клиента. Параметры каталога могут быть созданы на основе доступных Директорисеттингтемплатес, и значения, заданные по умолчанию, изменяются. Шаблоны параметров каталога невозможно создать, обновить или удалить. Эти параметры могут представлять параметры на уровне клиента или конкретные параметры сущности.  В настоящее время доступны только шаблоны для групп Office, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 73109edd383fe6f7d705f86f707c2096f8d9ac58
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340751"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="38815-107">Тип ресурса Директорисеттингтемплате</span><span class="sxs-lookup"><span data-stu-id="38815-107">directorySettingTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38815-108">Шаблоны параметров каталога представляют системные параметры, доступные для клиента.</span><span class="sxs-lookup"><span data-stu-id="38815-108">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="38815-109">[Параметры каталога](directorysetting.md) могут быть созданы на основе доступных директорисеттингтемплатес, и значения, заданные по умолчанию, изменяются.</span><span class="sxs-lookup"><span data-stu-id="38815-109">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="38815-110">Шаблоны параметров каталога невозможно создать, обновить или удалить.</span><span class="sxs-lookup"><span data-stu-id="38815-110">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="38815-111">Эти параметры могут представлять параметры на уровне клиента или конкретные параметры сущности.</span><span class="sxs-lookup"><span data-stu-id="38815-111">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="38815-112">В настоящее время доступны только шаблоны для групп Office, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.</span><span class="sxs-lookup"><span data-stu-id="38815-112">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="38815-113">**Note**: версия/Beta типа ресурса директорисеттингтемплате применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="38815-113">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="38815-114">Версия/v1.0 переименована в groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="38815-114">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="38815-115">Методы</span><span class="sxs-lookup"><span data-stu-id="38815-115">Methods</span></span>

| <span data-ttu-id="38815-116">Метод</span><span class="sxs-lookup"><span data-stu-id="38815-116">Method</span></span>           | <span data-ttu-id="38815-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="38815-117">Return Type</span></span>    |<span data-ttu-id="38815-118">Описание</span><span class="sxs-lookup"><span data-stu-id="38815-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="38815-119">Получение Директорисеттингтемплате</span><span class="sxs-lookup"><span data-stu-id="38815-119">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="38815-120">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="38815-120">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="38815-121">Чтение определенных свойств одного из системных объектов Директорисеттингтемплате, определенных системой.</span><span class="sxs-lookup"><span data-stu-id="38815-121">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="38815-122">Список Директорисеттингтемплате</span><span class="sxs-lookup"><span data-stu-id="38815-122">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="38815-123">Коллекция Директорисеттингтемплате</span><span class="sxs-lookup"><span data-stu-id="38815-123">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="38815-124">ПереЧисление всех объектов Директорисеттингтемплате, определенных системой.</span><span class="sxs-lookup"><span data-stu-id="38815-124">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="38815-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="38815-125">Properties</span></span>
| <span data-ttu-id="38815-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="38815-126">Property</span></span>     | <span data-ttu-id="38815-127">Тип</span><span class="sxs-lookup"><span data-stu-id="38815-127">Type</span></span>   |<span data-ttu-id="38815-128">Описание</span><span class="sxs-lookup"><span data-stu-id="38815-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38815-129">description</span><span class="sxs-lookup"><span data-stu-id="38815-129">description</span></span>|<span data-ttu-id="38815-130">string</span><span class="sxs-lookup"><span data-stu-id="38815-130">string</span></span>|<span data-ttu-id="38815-131">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="38815-131">Description of the template.</span></span> <span data-ttu-id="38815-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38815-132">Read-only.</span></span>|
|<span data-ttu-id="38815-133">displayName</span><span class="sxs-lookup"><span data-stu-id="38815-133">displayName</span></span>|<span data-ttu-id="38815-134">string</span><span class="sxs-lookup"><span data-stu-id="38815-134">string</span></span>|<span data-ttu-id="38815-135">Отображаемое имя шаблона.</span><span class="sxs-lookup"><span data-stu-id="38815-135">Display name of the template.</span></span> <span data-ttu-id="38815-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38815-136">Read-only.</span></span> |
|<span data-ttu-id="38815-137">id</span><span class="sxs-lookup"><span data-stu-id="38815-137">id</span></span>|<span data-ttu-id="38815-138">строка</span><span class="sxs-lookup"><span data-stu-id="38815-138">string</span></span>| <span data-ttu-id="38815-139">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="38815-139">Unique identifier for the template.</span></span> <span data-ttu-id="38815-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38815-140">Read-only.</span></span>|
|<span data-ttu-id="38815-141">values</span><span class="sxs-lookup"><span data-stu-id="38815-141">values</span></span>|<span data-ttu-id="38815-142">Коллекция [сеттингтемплатевалуе](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="38815-142">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="38815-143">Коллекция Settingtemplatevalue, в которой перечислены набор доступных параметров, значения по умолчанию и типы, которые составляют этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="38815-143">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="38815-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38815-144">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="38815-145">Отношения</span><span class="sxs-lookup"><span data-stu-id="38815-145">Relationships</span></span>
<span data-ttu-id="38815-146">Нет</span><span class="sxs-lookup"><span data-stu-id="38815-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="38815-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38815-147">JSON representation</span></span>

<span data-ttu-id="38815-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38815-148">Here is a JSON representation of the resource.</span></span>

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
