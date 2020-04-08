---
title: Тип ресурса Директорисеттингтемплате
description: Шаблоны параметров каталога представляют системные параметры, доступные для клиента.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 03803fddb12401e8d04318e8f4e7d7c63029b709
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181527"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="fb567-103">Тип ресурса Директорисеттингтемплате</span><span class="sxs-lookup"><span data-stu-id="fb567-103">directorySettingTemplate resource type</span></span>

<span data-ttu-id="fb567-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb567-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb567-105">Шаблоны параметров каталога представляют системные параметры, доступные для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb567-105">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="fb567-106">[Параметры каталога](directorysetting.md) могут быть созданы на основе доступных директорисеттингтемплатес, и значения, заданные по умолчанию, изменяются.</span><span class="sxs-lookup"><span data-stu-id="fb567-106">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="fb567-107">Шаблоны параметров каталога невозможно создать, обновить или удалить.</span><span class="sxs-lookup"><span data-stu-id="fb567-107">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="fb567-108">Эти параметры могут представлять параметры на уровне клиента или конкретные параметры сущности.</span><span class="sxs-lookup"><span data-stu-id="fb567-108">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="fb567-109">В настоящее время доступны только шаблоны для групп Office, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.</span><span class="sxs-lookup"><span data-stu-id="fb567-109">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="fb567-110">**Note**: версия/Beta типа ресурса директорисеттингтемплате применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="fb567-110">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="fb567-111">Версия/v1.0 переименована в groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="fb567-111">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="fb567-112">Методы</span><span class="sxs-lookup"><span data-stu-id="fb567-112">Methods</span></span>

| <span data-ttu-id="fb567-113">Метод</span><span class="sxs-lookup"><span data-stu-id="fb567-113">Method</span></span>           | <span data-ttu-id="fb567-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fb567-114">Return Type</span></span>    |<span data-ttu-id="fb567-115">Описание</span><span class="sxs-lookup"><span data-stu-id="fb567-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fb567-116">Получение Директорисеттингтемплате</span><span class="sxs-lookup"><span data-stu-id="fb567-116">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="fb567-117">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="fb567-117">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="fb567-118">Чтение определенных свойств одного из системных объектов Директорисеттингтемплате, определенных системой.</span><span class="sxs-lookup"><span data-stu-id="fb567-118">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="fb567-119">Список Директорисеттингтемплате</span><span class="sxs-lookup"><span data-stu-id="fb567-119">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="fb567-120">Коллекция Директорисеттингтемплате</span><span class="sxs-lookup"><span data-stu-id="fb567-120">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="fb567-121">Перечисление всех объектов Директорисеттингтемплате, определенных системой.</span><span class="sxs-lookup"><span data-stu-id="fb567-121">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="fb567-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb567-122">Properties</span></span>
| <span data-ttu-id="fb567-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb567-123">Property</span></span>     | <span data-ttu-id="fb567-124">Тип</span><span class="sxs-lookup"><span data-stu-id="fb567-124">Type</span></span>   |<span data-ttu-id="fb567-125">Описание</span><span class="sxs-lookup"><span data-stu-id="fb567-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb567-126">description</span><span class="sxs-lookup"><span data-stu-id="fb567-126">description</span></span>|<span data-ttu-id="fb567-127">string</span><span class="sxs-lookup"><span data-stu-id="fb567-127">string</span></span>|<span data-ttu-id="fb567-128">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="fb567-128">Description of the template.</span></span> <span data-ttu-id="fb567-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb567-129">Read-only.</span></span>|
|<span data-ttu-id="fb567-130">displayName</span><span class="sxs-lookup"><span data-stu-id="fb567-130">displayName</span></span>|<span data-ttu-id="fb567-131">string</span><span class="sxs-lookup"><span data-stu-id="fb567-131">string</span></span>|<span data-ttu-id="fb567-132">Отображаемое имя шаблона.</span><span class="sxs-lookup"><span data-stu-id="fb567-132">Display name of the template.</span></span> <span data-ttu-id="fb567-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb567-133">Read-only.</span></span> |
|<span data-ttu-id="fb567-134">id</span><span class="sxs-lookup"><span data-stu-id="fb567-134">id</span></span>|<span data-ttu-id="fb567-135">строка</span><span class="sxs-lookup"><span data-stu-id="fb567-135">string</span></span>| <span data-ttu-id="fb567-136">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="fb567-136">Unique identifier for the template.</span></span> <span data-ttu-id="fb567-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb567-137">Read-only.</span></span>|
|<span data-ttu-id="fb567-138">values</span><span class="sxs-lookup"><span data-stu-id="fb567-138">values</span></span>|<span data-ttu-id="fb567-139">Коллекция [сеттингтемплатевалуе](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="fb567-139">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="fb567-140">Коллекция Settingtemplatevalue, в которой перечислены набор доступных параметров, значения по умолчанию и типы, которые составляют этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="fb567-140">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="fb567-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb567-141">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fb567-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="fb567-142">Relationships</span></span>
<span data-ttu-id="fb567-143">Нет</span><span class="sxs-lookup"><span data-stu-id="fb567-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fb567-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb567-144">JSON representation</span></span>

<span data-ttu-id="fb567-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb567-145">Here is a JSON representation of the resource.</span></span>

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
