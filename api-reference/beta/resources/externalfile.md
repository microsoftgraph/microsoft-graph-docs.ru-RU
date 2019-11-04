---
title: Тип ресурса Екстерналфиле
description: Файл, индексируемый с помощью подключения Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bee1ad36769066550e1a6adc3ce7427602c66e66
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938985"
---
# <a name="externalfile-resource-type"></a><span data-ttu-id="65af8-103">Тип ресурса Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="65af8-103">externalFile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65af8-104">Элемент, индексируемый с помощью [подключения](externalconnection.md)поиска Microsoft.</span><span class="sxs-lookup"><span data-stu-id="65af8-104">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span> <span data-ttu-id="65af8-105">Этот тип является производным от типа [екстерналитем](externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="65af8-105">This type derives from the [externalItem](externalitem.md) type.</span></span>

## <a name="methods"></a><span data-ttu-id="65af8-106">Методы</span><span class="sxs-lookup"><span data-stu-id="65af8-106">Methods</span></span>

| <span data-ttu-id="65af8-107">Метод</span><span class="sxs-lookup"><span data-stu-id="65af8-107">Method</span></span>                                                        | <span data-ttu-id="65af8-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="65af8-108">Return Type</span></span>  | <span data-ttu-id="65af8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="65af8-109">Description</span></span> |
|:--------------------------------------------------------------|:-------------|:--|
| [<span data-ttu-id="65af8-110">Создание Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="65af8-110">Create externalFile</span></span>](../api/externalconnection-put-items.md) | <span data-ttu-id="65af8-111">екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="65af8-111">externalFile</span></span> | <span data-ttu-id="65af8-112">Создайте объект Екстерналфиле.</span><span class="sxs-lookup"><span data-stu-id="65af8-112">Create an externalFile.</span></span> |
| [<span data-ttu-id="65af8-113">Обновление Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="65af8-113">Update externalFile</span></span>](../api/externalitem-update.md)          | <span data-ttu-id="65af8-114">екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="65af8-114">externalFile</span></span> | <span data-ttu-id="65af8-115">Обновление Екстерналфиле.</span><span class="sxs-lookup"><span data-stu-id="65af8-115">Update an externalFile.</span></span> |
| [<span data-ttu-id="65af8-116">Delete</span><span class="sxs-lookup"><span data-stu-id="65af8-116">Delete</span></span>](../api/externalitem-delete.md)                       | <span data-ttu-id="65af8-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="65af8-117">None</span></span>         | <span data-ttu-id="65af8-118">Удаление Екстерналфиле.</span><span class="sxs-lookup"><span data-stu-id="65af8-118">Delete an externalFile.</span></span> |

## <a name="properties"></a><span data-ttu-id="65af8-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="65af8-119">Properties</span></span>

| <span data-ttu-id="65af8-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="65af8-120">Property</span></span>         | <span data-ttu-id="65af8-121">Тип</span><span class="sxs-lookup"><span data-stu-id="65af8-121">Type</span></span>                     | <span data-ttu-id="65af8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="65af8-122">Description</span></span>                    |
|:-----------------|:-------------------------|:-------------------------------|
| <span data-ttu-id="65af8-123">списки</span><span class="sxs-lookup"><span data-stu-id="65af8-123">acl</span></span>              | <span data-ttu-id="65af8-124">Коллекция [списков управления доступом](acl.md)</span><span class="sxs-lookup"><span data-stu-id="65af8-124">[acl](acl.md) collection</span></span> | <span data-ttu-id="65af8-125">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="65af8-125">An array of access control entries.</span></span> <span data-ttu-id="65af8-126">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="65af8-126">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="65af8-127">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="65af8-127">Required.</span></span> |
| <span data-ttu-id="65af8-128">content</span><span class="sxs-lookup"><span data-stu-id="65af8-128">content</span></span>          | <span data-ttu-id="65af8-129">String</span><span class="sxs-lookup"><span data-stu-id="65af8-129">String</span></span>                   | <span data-ttu-id="65af8-130">Представление содержимого элемента в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="65af8-130">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="65af8-131">Текст в этом свойстве является полнотекстовым индексированным.</span><span class="sxs-lookup"><span data-stu-id="65af8-131">The text in this property is full-text indexed.</span></span> <span data-ttu-id="65af8-132">Необязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="65af8-132">Optional.</span></span> |
| <span data-ttu-id="65af8-133">id</span><span class="sxs-lookup"><span data-stu-id="65af8-133">id</span></span>               | <span data-ttu-id="65af8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="65af8-134">String</span></span>                   | <span data-ttu-id="65af8-135">Предоставленный разработчиком уникальный идентификатор элемента в содержащем [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="65af8-135">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="65af8-136">Должен быть буквенно-цифровым и не превышать 128 символов.</span><span class="sxs-lookup"><span data-stu-id="65af8-136">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="65af8-137">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="65af8-137">Required.</span></span> |
| <span data-ttu-id="65af8-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="65af8-138">createdBy</span></span>        | <span data-ttu-id="65af8-139">Строка</span><span class="sxs-lookup"><span data-stu-id="65af8-139">String</span></span>                   | <span data-ttu-id="65af8-140">Имя пользователя, создавшего файл.</span><span class="sxs-lookup"><span data-stu-id="65af8-140">The name of the user that created the file.</span></span> |
| <span data-ttu-id="65af8-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65af8-141">createdDateTime</span></span>  | <span data-ttu-id="65af8-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65af8-142">DateTimeOffset</span></span>           | <span data-ttu-id="65af8-143">Дата и время создания файла.</span><span class="sxs-lookup"><span data-stu-id="65af8-143">The date and time that the file was created.</span></span> <span data-ttu-id="65af8-144">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="65af8-144">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="65af8-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="65af8-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="65af8-146">модулей</span><span class="sxs-lookup"><span data-stu-id="65af8-146">extension</span></span>        | <span data-ttu-id="65af8-147">Строка</span><span class="sxs-lookup"><span data-stu-id="65af8-147">String</span></span>                   | <span data-ttu-id="65af8-148">Расширение файла.</span><span class="sxs-lookup"><span data-stu-id="65af8-148">The file extension.</span></span>            |
| <span data-ttu-id="65af8-149">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="65af8-149">lastModifiedBy</span></span>   | <span data-ttu-id="65af8-150">Строка</span><span class="sxs-lookup"><span data-stu-id="65af8-150">String</span></span>                   | <span data-ttu-id="65af8-151">Имя пользователя, который последним изменил файл.</span><span class="sxs-lookup"><span data-stu-id="65af8-151">The name of the user that last modified the file.</span></span> |
| <span data-ttu-id="65af8-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65af8-152">modifiedDateTime</span></span> | <span data-ttu-id="65af8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65af8-153">DateTimeOffset</span></span>           | <span data-ttu-id="65af8-154">Дата и время последнего изменения файла.</span><span class="sxs-lookup"><span data-stu-id="65af8-154">The date and time that the file was last modified.</span></span> <span data-ttu-id="65af8-155">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="65af8-155">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="65af8-156">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="65af8-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="65af8-157">name</span><span class="sxs-lookup"><span data-stu-id="65af8-157">name</span></span>             | <span data-ttu-id="65af8-158">Строка</span><span class="sxs-lookup"><span data-stu-id="65af8-158">String</span></span>                   | <span data-ttu-id="65af8-159">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="65af8-159">The file name.</span></span> <span data-ttu-id="65af8-160">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="65af8-160">Required.</span></span>       |
| <span data-ttu-id="65af8-161">size</span><span class="sxs-lookup"><span data-stu-id="65af8-161">size</span></span>             | <span data-ttu-id="65af8-162">Int64</span><span class="sxs-lookup"><span data-stu-id="65af8-162">Int64</span></span>                    | <span data-ttu-id="65af8-163">Размер файла в байтах.</span><span class="sxs-lookup"><span data-stu-id="65af8-163">The size of the file in bytes.</span></span> |
| <span data-ttu-id="65af8-164">title</span><span class="sxs-lookup"><span data-stu-id="65af8-164">title</span></span>            | <span data-ttu-id="65af8-165">Строка</span><span class="sxs-lookup"><span data-stu-id="65af8-165">String</span></span>                   | <span data-ttu-id="65af8-166">Заголовок файла.</span><span class="sxs-lookup"><span data-stu-id="65af8-166">The title of the file.</span></span>         |
| <span data-ttu-id="65af8-167">url</span><span class="sxs-lookup"><span data-stu-id="65af8-167">url</span></span>              | <span data-ttu-id="65af8-168">Строка</span><span class="sxs-lookup"><span data-stu-id="65af8-168">String</span></span>                   | <span data-ttu-id="65af8-169">URL-адрес для доступа к файлу.</span><span class="sxs-lookup"><span data-stu-id="65af8-169">The URL to access the file.</span></span> <span data-ttu-id="65af8-170">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="65af8-170">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="65af8-171">Связи</span><span class="sxs-lookup"><span data-stu-id="65af8-171">Relationships</span></span>

<span data-ttu-id="65af8-172">Нет</span><span class="sxs-lookup"><span data-stu-id="65af8-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65af8-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65af8-173">JSON representation</span></span>

<span data-ttu-id="65af8-174">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65af8-174">The following is a JSON representation of the resource.</span></span>

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
