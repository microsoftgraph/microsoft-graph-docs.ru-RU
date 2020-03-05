---
title: Тип ресурса Екстерналфиле
description: Файл, индексируемый с помощью подключения Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 91de559bd365b9d6141e10a82af9ee06593f08ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498779"
---
# <a name="externalfile-resource-type"></a><span data-ttu-id="94457-103">Тип ресурса Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="94457-103">externalFile resource type</span></span>

<span data-ttu-id="94457-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="94457-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94457-105">Элемент, индексируемый с помощью [подключения](externalconnection.md)поиска Microsoft.</span><span class="sxs-lookup"><span data-stu-id="94457-105">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span> <span data-ttu-id="94457-106">Этот тип является производным от типа [екстерналитем](externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="94457-106">This type derives from the [externalItem](externalitem.md) type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="94457-107">Методы</span><span class="sxs-lookup"><span data-stu-id="94457-107">Methods</span></span>

| <span data-ttu-id="94457-108">Метод</span><span class="sxs-lookup"><span data-stu-id="94457-108">Method</span></span>                                                        | <span data-ttu-id="94457-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="94457-109">Return Type</span></span>  | <span data-ttu-id="94457-110">Описание</span><span class="sxs-lookup"><span data-stu-id="94457-110">Description</span></span> |
|:--------------------------------------------------------------|:-------------|:--|
| [<span data-ttu-id="94457-111">Создание Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="94457-111">Create externalFile</span></span>](../api/externalconnection-put-items.md) | <span data-ttu-id="94457-112">externalFile</span><span class="sxs-lookup"><span data-stu-id="94457-112">externalFile</span></span> | <span data-ttu-id="94457-113">Создайте объект Екстерналфиле.</span><span class="sxs-lookup"><span data-stu-id="94457-113">Create an externalFile.</span></span> |
| [<span data-ttu-id="94457-114">Обновление Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="94457-114">Update externalFile</span></span>](../api/externalitem-update.md)          | <span data-ttu-id="94457-115">externalFile</span><span class="sxs-lookup"><span data-stu-id="94457-115">externalFile</span></span> | <span data-ttu-id="94457-116">Обновление Екстерналфиле.</span><span class="sxs-lookup"><span data-stu-id="94457-116">Update an externalFile.</span></span> |
| <span data-ttu-id="94457-117">[удаление](../api/externalitem-delete.md);</span><span class="sxs-lookup"><span data-stu-id="94457-117">[Delete](../api/externalitem-delete.md)</span></span>                       | <span data-ttu-id="94457-118">Нет</span><span class="sxs-lookup"><span data-stu-id="94457-118">None</span></span>         | <span data-ttu-id="94457-119">Удаление Екстерналфиле.</span><span class="sxs-lookup"><span data-stu-id="94457-119">Delete an externalFile.</span></span> |

## <a name="properties"></a><span data-ttu-id="94457-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="94457-120">Properties</span></span>

| <span data-ttu-id="94457-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="94457-121">Property</span></span>         | <span data-ttu-id="94457-122">Тип</span><span class="sxs-lookup"><span data-stu-id="94457-122">Type</span></span>                     | <span data-ttu-id="94457-123">Описание</span><span class="sxs-lookup"><span data-stu-id="94457-123">Description</span></span>                    |
|:-----------------|:-------------------------|:-------------------------------|
| <span data-ttu-id="94457-124">списки</span><span class="sxs-lookup"><span data-stu-id="94457-124">acl</span></span>              | <span data-ttu-id="94457-125">Коллекция [списков управления доступом](acl.md)</span><span class="sxs-lookup"><span data-stu-id="94457-125">[acl](acl.md) collection</span></span> | <span data-ttu-id="94457-126">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="94457-126">An array of access control entries.</span></span> <span data-ttu-id="94457-127">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="94457-127">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="94457-128">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="94457-128">Required.</span></span> |
| <span data-ttu-id="94457-129">content</span><span class="sxs-lookup"><span data-stu-id="94457-129">content</span></span>          | <span data-ttu-id="94457-130">String</span><span class="sxs-lookup"><span data-stu-id="94457-130">String</span></span>                   | <span data-ttu-id="94457-131">Представление содержимого элемента в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="94457-131">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="94457-132">Текст в этом свойстве является полнотекстовым индексированным.</span><span class="sxs-lookup"><span data-stu-id="94457-132">The text in this property is full-text indexed.</span></span> <span data-ttu-id="94457-133">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="94457-133">Optional.</span></span> |
| <span data-ttu-id="94457-134">id</span><span class="sxs-lookup"><span data-stu-id="94457-134">id</span></span>               | <span data-ttu-id="94457-135">String</span><span class="sxs-lookup"><span data-stu-id="94457-135">String</span></span>                   | <span data-ttu-id="94457-136">Предоставленный разработчиком уникальный идентификатор элемента в содержащем [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="94457-136">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="94457-137">Должен быть буквенно-цифровым и не превышать 128 символов.</span><span class="sxs-lookup"><span data-stu-id="94457-137">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="94457-138">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="94457-138">Required.</span></span> |
| <span data-ttu-id="94457-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="94457-139">createdBy</span></span>        | <span data-ttu-id="94457-140">String</span><span class="sxs-lookup"><span data-stu-id="94457-140">String</span></span>                   | <span data-ttu-id="94457-141">Имя пользователя, создавшего файл.</span><span class="sxs-lookup"><span data-stu-id="94457-141">The name of the user that created the file.</span></span> |
| <span data-ttu-id="94457-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94457-142">createdDateTime</span></span>  | <span data-ttu-id="94457-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94457-143">DateTimeOffset</span></span>           | <span data-ttu-id="94457-144">Дата и время создания файла.</span><span class="sxs-lookup"><span data-stu-id="94457-144">The date and time that the file was created.</span></span> <span data-ttu-id="94457-145">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="94457-145">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="94457-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="94457-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="94457-147">модулей</span><span class="sxs-lookup"><span data-stu-id="94457-147">extension</span></span>        | <span data-ttu-id="94457-148">String</span><span class="sxs-lookup"><span data-stu-id="94457-148">String</span></span>                   | <span data-ttu-id="94457-149">Расширение файла.</span><span class="sxs-lookup"><span data-stu-id="94457-149">The file extension.</span></span>            |
| <span data-ttu-id="94457-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="94457-150">lastModifiedBy</span></span>   | <span data-ttu-id="94457-151">String</span><span class="sxs-lookup"><span data-stu-id="94457-151">String</span></span>                   | <span data-ttu-id="94457-152">Имя пользователя, который последним изменил файл.</span><span class="sxs-lookup"><span data-stu-id="94457-152">The name of the user that last modified the file.</span></span> |
| <span data-ttu-id="94457-153">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94457-153">modifiedDateTime</span></span> | <span data-ttu-id="94457-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94457-154">DateTimeOffset</span></span>           | <span data-ttu-id="94457-155">Дата и время последнего изменения файла.</span><span class="sxs-lookup"><span data-stu-id="94457-155">The date and time that the file was last modified.</span></span> <span data-ttu-id="94457-156">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="94457-156">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="94457-157">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="94457-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="94457-158">name</span><span class="sxs-lookup"><span data-stu-id="94457-158">name</span></span>             | <span data-ttu-id="94457-159">Строка</span><span class="sxs-lookup"><span data-stu-id="94457-159">String</span></span>                   | <span data-ttu-id="94457-160">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="94457-160">The file name.</span></span> <span data-ttu-id="94457-161">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="94457-161">Required.</span></span>       |
| <span data-ttu-id="94457-162">size</span><span class="sxs-lookup"><span data-stu-id="94457-162">size</span></span>             | <span data-ttu-id="94457-163">Int64</span><span class="sxs-lookup"><span data-stu-id="94457-163">Int64</span></span>                    | <span data-ttu-id="94457-164">Размер файла в байтах.</span><span class="sxs-lookup"><span data-stu-id="94457-164">The size of the file in bytes.</span></span> |
| <span data-ttu-id="94457-165">title</span><span class="sxs-lookup"><span data-stu-id="94457-165">title</span></span>            | <span data-ttu-id="94457-166">String</span><span class="sxs-lookup"><span data-stu-id="94457-166">String</span></span>                   | <span data-ttu-id="94457-167">Заголовок файла.</span><span class="sxs-lookup"><span data-stu-id="94457-167">The title of the file.</span></span>         |
| <span data-ttu-id="94457-168">url</span><span class="sxs-lookup"><span data-stu-id="94457-168">url</span></span>              | <span data-ttu-id="94457-169">String</span><span class="sxs-lookup"><span data-stu-id="94457-169">String</span></span>                   | <span data-ttu-id="94457-170">URL-адрес для доступа к файлу.</span><span class="sxs-lookup"><span data-stu-id="94457-170">The URL to access the file.</span></span> <span data-ttu-id="94457-171">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="94457-171">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="94457-172">Связи</span><span class="sxs-lookup"><span data-stu-id="94457-172">Relationships</span></span>

<span data-ttu-id="94457-173">Нет</span><span class="sxs-lookup"><span data-stu-id="94457-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94457-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94457-174">JSON representation</span></span>

<span data-ttu-id="94457-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94457-175">The following is a JSON representation of the resource.</span></span>

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
