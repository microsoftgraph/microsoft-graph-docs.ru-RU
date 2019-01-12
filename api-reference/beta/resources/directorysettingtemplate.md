---
title: Тип ресурса directorySettingTemplate
description: Шаблоны параметр Directory представляют системные параметры, доступные для клиента. Параметры каталога могут создаваться на основе доступных directorySettingTemplates и значения, измененные из предварительно значения по умолчанию. Шаблоны параметр каталога не создан, обновлении или удалении. Эти параметры можно представить параметры на уровне клиента или может представлять параметров определенной сущности.  На данный момент доступны только шаблоны применяются к группам Office и включают параметры, такие как пользователи могут создавать группы или пригласить Гости из за пределами организации стать членам группы.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d950b94c71bae70474bf9cdb9eee76fb8a3d9134
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957636"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="50bc2-107">Тип ресурса directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="50bc2-107">directorySettingTemplate resource type</span></span>

> <span data-ttu-id="50bc2-108">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="50bc2-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50bc2-109">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50bc2-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="50bc2-110">Шаблоны параметр Directory представляют системные параметры, доступные для клиента.</span><span class="sxs-lookup"><span data-stu-id="50bc2-110">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="50bc2-111">[Параметры каталога](directorysetting.md) могут создаваться на основе доступных directorySettingTemplates и значения, измененные из предварительно значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="50bc2-111">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="50bc2-112">Шаблоны параметр каталога не создан, обновлении или удалении.</span><span class="sxs-lookup"><span data-stu-id="50bc2-112">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="50bc2-113">Эти параметры можно представить параметры на уровне клиента или может представлять параметров определенной сущности.</span><span class="sxs-lookup"><span data-stu-id="50bc2-113">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="50bc2-114">На данный момент доступны только шаблоны применяются к группам Office и включают параметры, такие как пользователи могут создавать группы или пригласить Гости из за пределами организации стать членам группы.</span><span class="sxs-lookup"><span data-stu-id="50bc2-114">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="50bc2-115">**Примечание**: версия /beta типа ресурса directorySettingTemplate применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="50bc2-115">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="50bc2-116">Версия /v1.0 переименовано в groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="50bc2-116">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="50bc2-117">Методы</span><span class="sxs-lookup"><span data-stu-id="50bc2-117">Methods</span></span>

| <span data-ttu-id="50bc2-118">Метод</span><span class="sxs-lookup"><span data-stu-id="50bc2-118">Method</span></span>           | <span data-ttu-id="50bc2-119">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="50bc2-119">Return Type</span></span>    |<span data-ttu-id="50bc2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="50bc2-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="50bc2-121">Получение directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="50bc2-121">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="50bc2-122">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="50bc2-122">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="50bc2-123">Чтение определенных свойств объекта directorySettingTemplate определения системы.</span><span class="sxs-lookup"><span data-stu-id="50bc2-123">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="50bc2-124">Список directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="50bc2-124">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="50bc2-125">Коллекция directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="50bc2-125">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="50bc2-126">Список всех системных объектов directorySettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="50bc2-126">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="50bc2-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="50bc2-127">Properties</span></span>
| <span data-ttu-id="50bc2-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="50bc2-128">Property</span></span>     | <span data-ttu-id="50bc2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="50bc2-129">Type</span></span>   |<span data-ttu-id="50bc2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="50bc2-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50bc2-131">description</span><span class="sxs-lookup"><span data-stu-id="50bc2-131">description</span></span>|<span data-ttu-id="50bc2-132">строка</span><span class="sxs-lookup"><span data-stu-id="50bc2-132">string</span></span>|<span data-ttu-id="50bc2-133">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="50bc2-133">Description of the template.</span></span> <span data-ttu-id="50bc2-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50bc2-134">Read-only.</span></span>|
|<span data-ttu-id="50bc2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="50bc2-135">displayName</span></span>|<span data-ttu-id="50bc2-136">строка</span><span class="sxs-lookup"><span data-stu-id="50bc2-136">string</span></span>|<span data-ttu-id="50bc2-137">Отображаемое имя шаблона.</span><span class="sxs-lookup"><span data-stu-id="50bc2-137">Display name of the template.</span></span> <span data-ttu-id="50bc2-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50bc2-138">Read-only.</span></span> |
|<span data-ttu-id="50bc2-139">id</span><span class="sxs-lookup"><span data-stu-id="50bc2-139">id</span></span>|<span data-ttu-id="50bc2-140">строка</span><span class="sxs-lookup"><span data-stu-id="50bc2-140">string</span></span>| <span data-ttu-id="50bc2-p107">Уникальный идентификатор шаблона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50bc2-p107">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="50bc2-143">values</span><span class="sxs-lookup"><span data-stu-id="50bc2-143">values</span></span>|<span data-ttu-id="50bc2-144">Коллекция объектов [settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="50bc2-144">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="50bc2-145">Коллекция объектов settingTemplateValue, перечисляющих набор доступных параметров, значений по умолчанию и типов, которые составляют шаблон.</span><span class="sxs-lookup"><span data-stu-id="50bc2-145">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="50bc2-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50bc2-146">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="50bc2-147">Связи</span><span class="sxs-lookup"><span data-stu-id="50bc2-147">Relationships</span></span>
<span data-ttu-id="50bc2-148">Нет</span><span class="sxs-lookup"><span data-stu-id="50bc2-148">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="50bc2-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50bc2-149">JSON representation</span></span>

<span data-ttu-id="50bc2-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50bc2-150">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
