---
title: Тип ресурса Директорисеттингтемплате
description: Шаблоны параметров каталога представляют системные параметры, доступные для клиента. Параметры каталога могут быть созданы на основе доступных Директорисеттингтемплатес, и значения, заданные по умолчанию, изменяются. Шаблоны параметров каталога невозможно создать, обновить или удалить. Эти параметры могут представлять параметры на уровне клиента или конкретные параметры сущности.  В настоящее время доступны только шаблоны для групп Office, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f1881c697eae6b4032635d2e4797a14ef2e848e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42506465"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="29abe-107">Тип ресурса Директорисеттингтемплате</span><span class="sxs-lookup"><span data-stu-id="29abe-107">directorySettingTemplate resource type</span></span>

<span data-ttu-id="29abe-108">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="29abe-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29abe-109">Шаблоны параметров каталога представляют системные параметры, доступные для клиента.</span><span class="sxs-lookup"><span data-stu-id="29abe-109">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="29abe-110">[Параметры каталога](directorysetting.md) могут быть созданы на основе доступных директорисеттингтемплатес, и значения, заданные по умолчанию, изменяются.</span><span class="sxs-lookup"><span data-stu-id="29abe-110">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="29abe-111">Шаблоны параметров каталога невозможно создать, обновить или удалить.</span><span class="sxs-lookup"><span data-stu-id="29abe-111">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="29abe-112">Эти параметры могут представлять параметры на уровне клиента или конкретные параметры сущности.</span><span class="sxs-lookup"><span data-stu-id="29abe-112">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="29abe-113">В настоящее время доступны только шаблоны для групп Office, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.</span><span class="sxs-lookup"><span data-stu-id="29abe-113">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="29abe-114">**Note**: версия/Beta типа ресурса директорисеттингтемплате применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="29abe-114">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="29abe-115">Версия/v1.0 переименована в groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="29abe-115">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="29abe-116">Методы</span><span class="sxs-lookup"><span data-stu-id="29abe-116">Methods</span></span>

| <span data-ttu-id="29abe-117">Метод</span><span class="sxs-lookup"><span data-stu-id="29abe-117">Method</span></span>           | <span data-ttu-id="29abe-118">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="29abe-118">Return Type</span></span>    |<span data-ttu-id="29abe-119">Описание</span><span class="sxs-lookup"><span data-stu-id="29abe-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="29abe-120">Получение Директорисеттингтемплате</span><span class="sxs-lookup"><span data-stu-id="29abe-120">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="29abe-121">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="29abe-121">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="29abe-122">Чтение определенных свойств одного из системных объектов Директорисеттингтемплате, определенных системой.</span><span class="sxs-lookup"><span data-stu-id="29abe-122">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="29abe-123">Список Директорисеттингтемплате</span><span class="sxs-lookup"><span data-stu-id="29abe-123">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="29abe-124">Коллекция Директорисеттингтемплате</span><span class="sxs-lookup"><span data-stu-id="29abe-124">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="29abe-125">Перечисление всех объектов Директорисеттингтемплате, определенных системой.</span><span class="sxs-lookup"><span data-stu-id="29abe-125">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="29abe-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="29abe-126">Properties</span></span>
| <span data-ttu-id="29abe-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="29abe-127">Property</span></span>     | <span data-ttu-id="29abe-128">Тип</span><span class="sxs-lookup"><span data-stu-id="29abe-128">Type</span></span>   |<span data-ttu-id="29abe-129">Описание</span><span class="sxs-lookup"><span data-stu-id="29abe-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29abe-130">description</span><span class="sxs-lookup"><span data-stu-id="29abe-130">description</span></span>|<span data-ttu-id="29abe-131">string</span><span class="sxs-lookup"><span data-stu-id="29abe-131">string</span></span>|<span data-ttu-id="29abe-132">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="29abe-132">Description of the template.</span></span> <span data-ttu-id="29abe-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29abe-133">Read-only.</span></span>|
|<span data-ttu-id="29abe-134">displayName</span><span class="sxs-lookup"><span data-stu-id="29abe-134">displayName</span></span>|<span data-ttu-id="29abe-135">string</span><span class="sxs-lookup"><span data-stu-id="29abe-135">string</span></span>|<span data-ttu-id="29abe-136">Отображаемое имя шаблона.</span><span class="sxs-lookup"><span data-stu-id="29abe-136">Display name of the template.</span></span> <span data-ttu-id="29abe-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29abe-137">Read-only.</span></span> |
|<span data-ttu-id="29abe-138">id</span><span class="sxs-lookup"><span data-stu-id="29abe-138">id</span></span>|<span data-ttu-id="29abe-139">строка</span><span class="sxs-lookup"><span data-stu-id="29abe-139">string</span></span>| <span data-ttu-id="29abe-140">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="29abe-140">Unique identifier for the template.</span></span> <span data-ttu-id="29abe-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29abe-141">Read-only.</span></span>|
|<span data-ttu-id="29abe-142">values</span><span class="sxs-lookup"><span data-stu-id="29abe-142">values</span></span>|<span data-ttu-id="29abe-143">Коллекция [сеттингтемплатевалуе](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="29abe-143">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="29abe-144">Коллекция Settingtemplatevalue, в которой перечислены набор доступных параметров, значения по умолчанию и типы, которые составляют этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="29abe-144">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="29abe-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29abe-145">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="29abe-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="29abe-146">Relationships</span></span>
<span data-ttu-id="29abe-147">Нет</span><span class="sxs-lookup"><span data-stu-id="29abe-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="29abe-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29abe-148">JSON representation</span></span>

<span data-ttu-id="29abe-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29abe-149">Here is a JSON representation of the resource.</span></span>

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
