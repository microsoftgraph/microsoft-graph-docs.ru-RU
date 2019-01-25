---
title: Тип ресурса directorySettingTemplate
description: Шаблоны параметр Directory представляют системные параметры, доступные для клиента. Параметры каталога могут создаваться на основе доступных directorySettingTemplates и значения, измененные из предварительно значения по умолчанию. Шаблоны параметр каталога не создан, обновлении или удалении. Эти параметры можно представить параметры на уровне клиента или может представлять параметров определенной сущности.  На данный момент доступны только шаблоны применяются к группам Office и включают параметры, такие как пользователи могут создавать группы или пригласить Гости из за пределами организации стать членам группы.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 366817df422686a8db658f1cab1d5805c24c4f91
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516660"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="f0960-107">Тип ресурса directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="f0960-107">directorySettingTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0960-108">Шаблоны параметр Directory представляют системные параметры, доступные для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0960-108">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="f0960-109">[Параметры каталога](directorysetting.md) могут создаваться на основе доступных directorySettingTemplates и значения, измененные из предварительно значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f0960-109">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="f0960-110">Шаблоны параметр каталога не создан, обновлении или удалении.</span><span class="sxs-lookup"><span data-stu-id="f0960-110">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="f0960-111">Эти параметры можно представить параметры на уровне клиента или может представлять параметров определенной сущности.</span><span class="sxs-lookup"><span data-stu-id="f0960-111">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="f0960-112">На данный момент доступны только шаблоны применяются к группам Office и включают параметры, такие как пользователи могут создавать группы или пригласить Гости из за пределами организации стать членам группы.</span><span class="sxs-lookup"><span data-stu-id="f0960-112">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="f0960-113">**Примечание**: версия /beta типа ресурса directorySettingTemplate применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="f0960-113">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="f0960-114">Версия /v1.0 переименовано в groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="f0960-114">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="f0960-115">Методы</span><span class="sxs-lookup"><span data-stu-id="f0960-115">Methods</span></span>

| <span data-ttu-id="f0960-116">Метод</span><span class="sxs-lookup"><span data-stu-id="f0960-116">Method</span></span>           | <span data-ttu-id="f0960-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f0960-117">Return Type</span></span>    |<span data-ttu-id="f0960-118">Описание</span><span class="sxs-lookup"><span data-stu-id="f0960-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f0960-119">Получение directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="f0960-119">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="f0960-120">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="f0960-120">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="f0960-121">Чтение определенных свойств объекта directorySettingTemplate определения системы.</span><span class="sxs-lookup"><span data-stu-id="f0960-121">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="f0960-122">Список directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="f0960-122">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="f0960-123">Коллекция directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="f0960-123">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="f0960-124">Список всех системных объектов directorySettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="f0960-124">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="f0960-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0960-125">Properties</span></span>
| <span data-ttu-id="f0960-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0960-126">Property</span></span>     | <span data-ttu-id="f0960-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f0960-127">Type</span></span>   |<span data-ttu-id="f0960-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f0960-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0960-129">description</span><span class="sxs-lookup"><span data-stu-id="f0960-129">description</span></span>|<span data-ttu-id="f0960-130">строка</span><span class="sxs-lookup"><span data-stu-id="f0960-130">string</span></span>|<span data-ttu-id="f0960-131">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="f0960-131">Description of the template.</span></span> <span data-ttu-id="f0960-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0960-132">Read-only.</span></span>|
|<span data-ttu-id="f0960-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f0960-133">displayName</span></span>|<span data-ttu-id="f0960-134">string</span><span class="sxs-lookup"><span data-stu-id="f0960-134">string</span></span>|<span data-ttu-id="f0960-135">Отображаемое имя шаблона.</span><span class="sxs-lookup"><span data-stu-id="f0960-135">Display name of the template.</span></span> <span data-ttu-id="f0960-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0960-136">Read-only.</span></span> |
|<span data-ttu-id="f0960-137">id</span><span class="sxs-lookup"><span data-stu-id="f0960-137">id</span></span>|<span data-ttu-id="f0960-138">string</span><span class="sxs-lookup"><span data-stu-id="f0960-138">string</span></span>| <span data-ttu-id="f0960-p106">Уникальный идентификатор шаблона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0960-p106">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="f0960-141">values</span><span class="sxs-lookup"><span data-stu-id="f0960-141">values</span></span>|<span data-ttu-id="f0960-142">Коллекция объектов [settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="f0960-142">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="f0960-143">Коллекция объектов settingTemplateValue, перечисляющих набор доступных параметров, значений по умолчанию и типов, которые составляют шаблон.</span><span class="sxs-lookup"><span data-stu-id="f0960-143">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="f0960-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0960-144">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f0960-145">Отношения</span><span class="sxs-lookup"><span data-stu-id="f0960-145">Relationships</span></span>
<span data-ttu-id="f0960-146">Нет</span><span class="sxs-lookup"><span data-stu-id="f0960-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f0960-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0960-147">JSON representation</span></span>

<span data-ttu-id="f0960-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0960-148">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysettingtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
