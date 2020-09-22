---
title: Тип ресурса Екстерналфиле
description: Файл, индексируемый с помощью подключения Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 90faf3b10d09e84c9c0571d01fc242464888ff1e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071250"
---
# <a name="externalfile-resource-type"></a><span data-ttu-id="3b2e4-103">Тип ресурса Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="3b2e4-103">externalFile resource type</span></span>

<span data-ttu-id="3b2e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b2e4-104">Namespace: microsoft.graph</span></span>

> [!CAUTION]
> <span data-ttu-id="3b2e4-105">`externalFile`Тип устарел.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-105">The `externalFile` type has been deprecated.</span></span> <span data-ttu-id="3b2e4-106">Разработчикам не следует использовать этот тип.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-106">Developers should not use this type.</span></span> <span data-ttu-id="3b2e4-107">Внешние файлы по-прежнему могут индексироваться с помощью типа [екстерналитем](externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="3b2e4-107">External files may still be indexed using the [externalItem](externalitem.md) type.</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b2e4-108">Элемент, индексируемый с помощью [подключения](externalconnection.md)поиска Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-108">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span> <span data-ttu-id="3b2e4-109">Этот тип является производным от типа [екстерналитем](externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="3b2e4-109">This type derives from the [externalItem](externalitem.md) type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="3b2e4-110">Методы</span><span class="sxs-lookup"><span data-stu-id="3b2e4-110">Methods</span></span>

| <span data-ttu-id="3b2e4-111">Метод</span><span class="sxs-lookup"><span data-stu-id="3b2e4-111">Method</span></span>                                                        | <span data-ttu-id="3b2e4-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3b2e4-112">Return Type</span></span>  | <span data-ttu-id="3b2e4-113">Описание</span><span class="sxs-lookup"><span data-stu-id="3b2e4-113">Description</span></span> |
|:--------------------------------------------------------------|:-------------|:--|
| [<span data-ttu-id="3b2e4-114">Создание Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="3b2e4-114">Create externalFile</span></span>](../api/externalconnection-put-items.md) | <span data-ttu-id="3b2e4-115">externalFile</span><span class="sxs-lookup"><span data-stu-id="3b2e4-115">externalFile</span></span> | <span data-ttu-id="3b2e4-116">Создайте объект Екстерналфиле.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-116">Create an externalFile.</span></span> |
| [<span data-ttu-id="3b2e4-117">Обновление Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="3b2e4-117">Update externalFile</span></span>](../api/externalitem-update.md)          | <span data-ttu-id="3b2e4-118">externalFile</span><span class="sxs-lookup"><span data-stu-id="3b2e4-118">externalFile</span></span> | <span data-ttu-id="3b2e4-119">Обновление Екстерналфиле.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-119">Update an externalFile.</span></span> |
| [<span data-ttu-id="3b2e4-120">Удаление</span><span class="sxs-lookup"><span data-stu-id="3b2e4-120">Delete</span></span>](../api/externalitem-delete.md)                       | <span data-ttu-id="3b2e4-121">Нет</span><span class="sxs-lookup"><span data-stu-id="3b2e4-121">None</span></span>         | <span data-ttu-id="3b2e4-122">Удаление Екстерналфиле.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-122">Delete an externalFile.</span></span> |

## <a name="properties"></a><span data-ttu-id="3b2e4-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b2e4-123">Properties</span></span>

| <span data-ttu-id="3b2e4-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b2e4-124">Property</span></span>         | <span data-ttu-id="3b2e4-125">Тип</span><span class="sxs-lookup"><span data-stu-id="3b2e4-125">Type</span></span>                     | <span data-ttu-id="3b2e4-126">Описание</span><span class="sxs-lookup"><span data-stu-id="3b2e4-126">Description</span></span>                    |
|:-----------------|:-------------------------|:-------------------------------|
| <span data-ttu-id="3b2e4-127">списки</span><span class="sxs-lookup"><span data-stu-id="3b2e4-127">acl</span></span>              | <span data-ttu-id="3b2e4-128">Коллекция [списков управления доступом](acl.md)</span><span class="sxs-lookup"><span data-stu-id="3b2e4-128">[acl](acl.md) collection</span></span> | <span data-ttu-id="3b2e4-129">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-129">An array of access control entries.</span></span> <span data-ttu-id="3b2e4-130">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-130">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="3b2e4-131">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-131">Required.</span></span> |
| <span data-ttu-id="3b2e4-132">content</span><span class="sxs-lookup"><span data-stu-id="3b2e4-132">content</span></span>          | <span data-ttu-id="3b2e4-133">String</span><span class="sxs-lookup"><span data-stu-id="3b2e4-133">String</span></span>                   | <span data-ttu-id="3b2e4-134">Представление содержимого элемента в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-134">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="3b2e4-135">Текст в этом свойстве является полнотекстовым индексированным.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-135">The text in this property is full-text indexed.</span></span> <span data-ttu-id="3b2e4-136">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-136">Optional.</span></span> |
| <span data-ttu-id="3b2e4-137">id</span><span class="sxs-lookup"><span data-stu-id="3b2e4-137">id</span></span>               | <span data-ttu-id="3b2e4-138">String</span><span class="sxs-lookup"><span data-stu-id="3b2e4-138">String</span></span>                   | <span data-ttu-id="3b2e4-139">Предоставленный разработчиком уникальный идентификатор элемента в содержащем [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="3b2e4-139">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="3b2e4-140">Должен быть буквенно-цифровым и не превышать 128 символов.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-140">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="3b2e4-141">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-141">Required.</span></span> |
| <span data-ttu-id="3b2e4-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="3b2e4-142">createdBy</span></span>        | <span data-ttu-id="3b2e4-143">String</span><span class="sxs-lookup"><span data-stu-id="3b2e4-143">String</span></span>                   | <span data-ttu-id="3b2e4-144">Имя пользователя, создавшего файл.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-144">The name of the user that created the file.</span></span> |
| <span data-ttu-id="3b2e4-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b2e4-145">createdDateTime</span></span>  | <span data-ttu-id="3b2e4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b2e4-146">DateTimeOffset</span></span>           | <span data-ttu-id="3b2e4-147">Дата и время создания файла.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-147">The date and time that the file was created.</span></span> <span data-ttu-id="3b2e4-148">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-148">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3b2e4-149">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="3b2e4-150">модулей</span><span class="sxs-lookup"><span data-stu-id="3b2e4-150">extension</span></span>        | <span data-ttu-id="3b2e4-151">String</span><span class="sxs-lookup"><span data-stu-id="3b2e4-151">String</span></span>                   | <span data-ttu-id="3b2e4-152">Расширение файла.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-152">The file extension.</span></span>            |
| <span data-ttu-id="3b2e4-153">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="3b2e4-153">lastModifiedBy</span></span>   | <span data-ttu-id="3b2e4-154">String</span><span class="sxs-lookup"><span data-stu-id="3b2e4-154">String</span></span>                   | <span data-ttu-id="3b2e4-155">Имя пользователя, который последним изменил файл.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-155">The name of the user that last modified the file.</span></span> |
| <span data-ttu-id="3b2e4-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b2e4-156">modifiedDateTime</span></span> | <span data-ttu-id="3b2e4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b2e4-157">DateTimeOffset</span></span>           | <span data-ttu-id="3b2e4-158">Дата и время последнего изменения файла.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-158">The date and time that the file was last modified.</span></span> <span data-ttu-id="3b2e4-159">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-159">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3b2e4-160">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-160">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="3b2e4-161">name</span><span class="sxs-lookup"><span data-stu-id="3b2e4-161">name</span></span>             | <span data-ttu-id="3b2e4-162">String</span><span class="sxs-lookup"><span data-stu-id="3b2e4-162">String</span></span>                   | <span data-ttu-id="3b2e4-163">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-163">The file name.</span></span> <span data-ttu-id="3b2e4-164">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-164">Required.</span></span>       |
| <span data-ttu-id="3b2e4-165">size</span><span class="sxs-lookup"><span data-stu-id="3b2e4-165">size</span></span>             | <span data-ttu-id="3b2e4-166">Int64</span><span class="sxs-lookup"><span data-stu-id="3b2e4-166">Int64</span></span>                    | <span data-ttu-id="3b2e4-167">Размер файла в байтах.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-167">The size of the file in bytes.</span></span> |
| <span data-ttu-id="3b2e4-168">title</span><span class="sxs-lookup"><span data-stu-id="3b2e4-168">title</span></span>            | <span data-ttu-id="3b2e4-169">String</span><span class="sxs-lookup"><span data-stu-id="3b2e4-169">String</span></span>                   | <span data-ttu-id="3b2e4-170">Заголовок файла.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-170">The title of the file.</span></span>         |
| <span data-ttu-id="3b2e4-171">url</span><span class="sxs-lookup"><span data-stu-id="3b2e4-171">url</span></span>              | <span data-ttu-id="3b2e4-172">String</span><span class="sxs-lookup"><span data-stu-id="3b2e4-172">String</span></span>                   | <span data-ttu-id="3b2e4-173">URL-адрес для доступа к файлу.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-173">The URL to access the file.</span></span> <span data-ttu-id="3b2e4-174">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-174">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3b2e4-175">Отношения</span><span class="sxs-lookup"><span data-stu-id="3b2e4-175">Relationships</span></span>

<span data-ttu-id="3b2e4-176">Нет</span><span class="sxs-lookup"><span data-stu-id="3b2e4-176">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b2e4-177">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b2e4-177">JSON representation</span></span>

<span data-ttu-id="3b2e4-178">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b2e4-178">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalFile",
  "baseType": "microsoft.graph.externalItem"
}-->

```json
{
  "acl": [{"@odata.type": "microsoft.graph.acl"}],
  "content": "String",
  "id": "String (identifier)",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "extension": "String",
  "lastModifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "title": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


