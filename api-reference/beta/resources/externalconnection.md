---
title: Тип ресурса Екстерналконнектион
description: Подключение — это логический контейнер для внешнего контента в Microsoft Graph.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 82a68c8670a1381263d0b6fd3704f9d6d900d1f0
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193143"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="4ea11-103">Тип ресурса Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="4ea11-103">externalConnection resource type</span></span>

<span data-ttu-id="4ea11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ea11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ea11-105">Логический контейнер для добавления контента из внешнего источника в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4ea11-105">A logical container to add content from an external source into Microsoft Graph.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="4ea11-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4ea11-106">Methods</span></span>

| <span data-ttu-id="4ea11-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4ea11-107">Method</span></span>                                                           | <span data-ttu-id="4ea11-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4ea11-108">Return Type</span></span>                                   | <span data-ttu-id="4ea11-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4ea11-109">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="4ea11-110">Создание Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="4ea11-110">Create externalConnection</span></span>](../api/external-post-connections.md) | <span data-ttu-id="4ea11-111">externalConnection</span><span class="sxs-lookup"><span data-stu-id="4ea11-111">externalConnection</span></span>                            | <span data-ttu-id="4ea11-112">Создание нового Екстерналконнектион путем публикации в коллекции Connections.</span><span class="sxs-lookup"><span data-stu-id="4ea11-112">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="4ea11-113">Список Екстерналконнектионс</span><span class="sxs-lookup"><span data-stu-id="4ea11-113">List externalConnections</span></span>](../api/externalconnection-list.md)    | <span data-ttu-id="4ea11-114">Коллекция Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="4ea11-114">externalConnection collection</span></span>                 | <span data-ttu-id="4ea11-115">Получение коллекции объектов Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="4ea11-115">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="4ea11-116">Получение Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="4ea11-116">Get externalConnection</span></span>](../api/externalconnection-get.md)       | <span data-ttu-id="4ea11-117">externalConnection</span><span class="sxs-lookup"><span data-stu-id="4ea11-117">externalConnection</span></span>                            | <span data-ttu-id="4ea11-118">Чтение свойств и связей объекта Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="4ea11-118">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="4ea11-119">Обновление Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="4ea11-119">Update externalConnection</span></span>](../api/externalconnection-update.md) | <span data-ttu-id="4ea11-120">externalConnection</span><span class="sxs-lookup"><span data-stu-id="4ea11-120">externalConnection</span></span>                            | <span data-ttu-id="4ea11-121">Обновление объекта Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="4ea11-121">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="4ea11-122">Удаление Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="4ea11-122">Delete externalConnection</span></span>](../api/externalconnection-delete.md) | <span data-ttu-id="4ea11-123">Нет</span><span class="sxs-lookup"><span data-stu-id="4ea11-123">None</span></span>                                          | <span data-ttu-id="4ea11-124">Удаление объекта Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="4ea11-124">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="4ea11-125">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="4ea11-125">Create schema</span></span>](../api/externalconnection-post-schema.md)        | <span data-ttu-id="4ea11-126">Нет *или* [схема](schema.md)</span><span class="sxs-lookup"><span data-stu-id="4ea11-126">None *or* [schema](schema.md)</span></span>                 | <span data-ttu-id="4ea11-127">Регистрация схемы подключения.</span><span class="sxs-lookup"><span data-stu-id="4ea11-127">Register connection schema.</span></span> |
| [<span data-ttu-id="4ea11-128">Получение операции</span><span class="sxs-lookup"><span data-stu-id="4ea11-128">Get operation</span></span>](../api/connectionoperation-get.md)               | [<span data-ttu-id="4ea11-129">коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="4ea11-129">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="4ea11-130">Получение состояния асинхронного запроса для создания схемы подключения.</span><span class="sxs-lookup"><span data-stu-id="4ea11-130">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="4ea11-131">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="4ea11-131">Create externalItem</span></span>](../api/externalconnection-put-items.md)    | [<span data-ttu-id="4ea11-132">externalItem</span><span class="sxs-lookup"><span data-stu-id="4ea11-132">externalItem</span></span>](externalitem.md)               | <span data-ttu-id="4ea11-133">Создание нового Екстерналитем путем публикации в коллекции Items.</span><span class="sxs-lookup"><span data-stu-id="4ea11-133">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="4ea11-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ea11-134">Properties</span></span>

| <span data-ttu-id="4ea11-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ea11-135">Property</span></span>      | <span data-ttu-id="4ea11-136">Тип</span><span class="sxs-lookup"><span data-stu-id="4ea11-136">Type</span></span>                              | <span data-ttu-id="4ea11-137">Описание</span><span class="sxs-lookup"><span data-stu-id="4ea11-137">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="4ea11-138">configuration</span><span class="sxs-lookup"><span data-stu-id="4ea11-138">configuration</span></span> | [<span data-ttu-id="4ea11-139">configuration</span><span class="sxs-lookup"><span data-stu-id="4ea11-139">configuration</span></span>](configuration.md) | <span data-ttu-id="4ea11-140">Задает дополнительные идентификаторы приложений, которым разрешено управлять подключением и индексировать содержимое в подключении.</span><span class="sxs-lookup"><span data-stu-id="4ea11-140">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="4ea11-141">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="4ea11-141">Optional.</span></span> |
| <span data-ttu-id="4ea11-142">description</span><span class="sxs-lookup"><span data-stu-id="4ea11-142">description</span></span>   | <span data-ttu-id="4ea11-143">String</span><span class="sxs-lookup"><span data-stu-id="4ea11-143">String</span></span>                            | <span data-ttu-id="4ea11-144">Описание подключения, отображаемое в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4ea11-144">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="4ea11-145">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="4ea11-145">Optional.</span></span> |
| <span data-ttu-id="4ea11-146">id</span><span class="sxs-lookup"><span data-stu-id="4ea11-146">id</span></span>            | <span data-ttu-id="4ea11-147">String</span><span class="sxs-lookup"><span data-stu-id="4ea11-147">String</span></span>                            | <span data-ttu-id="4ea11-148">Предоставленный разработчиком уникальный идентификатор подключения в клиенте Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4ea11-148">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="4ea11-149">Максимальная длина 32 символов.</span><span class="sxs-lookup"><span data-stu-id="4ea11-149">Maximum length of 32 characters.</span></span> <span data-ttu-id="4ea11-150">Должно содержать только буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="4ea11-150">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="4ea11-151">Не может начинаться с `Microsoft` одного из следующих значений:,,,,,,,,,, `None` `Directory` `Exchange` `ExchangeArchive` `LinkedIn` `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` , `Connectors` .</span><span class="sxs-lookup"><span data-stu-id="4ea11-151">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`.</span></span> <span data-ttu-id="4ea11-152">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4ea11-152">Required.</span></span> |
| <span data-ttu-id="4ea11-153">name</span><span class="sxs-lookup"><span data-stu-id="4ea11-153">name</span></span>          | <span data-ttu-id="4ea11-154">String</span><span class="sxs-lookup"><span data-stu-id="4ea11-154">String</span></span>                            | <span data-ttu-id="4ea11-155">Отображаемое имя подключения, отображаемое в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4ea11-155">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="4ea11-156">Максимальная длина 128 символов.</span><span class="sxs-lookup"><span data-stu-id="4ea11-156">Maximum length of 128 characters.</span></span> <span data-ttu-id="4ea11-157">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4ea11-157">Required.</span></span> |
| <span data-ttu-id="4ea11-158">state</span><span class="sxs-lookup"><span data-stu-id="4ea11-158">state</span></span>         | <span data-ttu-id="4ea11-159">коннектионстате</span><span class="sxs-lookup"><span data-stu-id="4ea11-159">connectionState</span></span>                   | <span data-ttu-id="4ea11-160">Указывает текущее состояние подключения.</span><span class="sxs-lookup"><span data-stu-id="4ea11-160">Indicates the current state of the connection.</span></span> <span data-ttu-id="4ea11-161">Возможные значения: `draft` , `ready` , `obsolete` и `limitExceeded` .</span><span class="sxs-lookup"><span data-stu-id="4ea11-161">Possible values are `draft`, `ready`, `obsolete`, and `limitExceeded`.</span></span> <span data-ttu-id="4ea11-162">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ea11-162">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4ea11-163">Связи</span><span class="sxs-lookup"><span data-stu-id="4ea11-163">Relationships</span></span>

| <span data-ttu-id="4ea11-164">Связь</span><span class="sxs-lookup"><span data-stu-id="4ea11-164">Relationship</span></span> | <span data-ttu-id="4ea11-165">Тип</span><span class="sxs-lookup"><span data-stu-id="4ea11-165">Type</span></span>                                                     | <span data-ttu-id="4ea11-166">Описание</span><span class="sxs-lookup"><span data-stu-id="4ea11-166">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="4ea11-167">items</span><span class="sxs-lookup"><span data-stu-id="4ea11-167">items</span></span>        | <span data-ttu-id="4ea11-168">Коллекция [екстерналитем](externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="4ea11-168">[externalItem](externalitem.md) collection</span></span>               | <span data-ttu-id="4ea11-p106">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4ea11-p106">Read-only. Nullable.</span></span> |
| <span data-ttu-id="4ea11-171">operations</span><span class="sxs-lookup"><span data-stu-id="4ea11-171">operations</span></span>   | <span data-ttu-id="4ea11-172">Коллекция [коннектионоператион](connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="4ea11-172">[connectionOperation](connectionoperation.md) collection</span></span> | <span data-ttu-id="4ea11-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ea11-173">Read-only.</span></span> <span data-ttu-id="4ea11-174">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4ea11-174">Nullable.</span></span> |
| <span data-ttu-id="4ea11-175">схемы</span><span class="sxs-lookup"><span data-stu-id="4ea11-175">schema</span></span>       | [<span data-ttu-id="4ea11-176">schema</span><span class="sxs-lookup"><span data-stu-id="4ea11-176">schema</span></span>](schema.md)                                      | <span data-ttu-id="4ea11-p108">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4ea11-p108">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4ea11-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ea11-179">JSON representation</span></span>

<span data-ttu-id="4ea11-180">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ea11-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnection",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "configuration": {"@odata.type": "microsoft.graph.configuration"},
  "description": "String",
  "id": "String (identifier)",
  "name": "String",
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
