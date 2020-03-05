---
title: Тип ресурса Екстерналконнектион
description: Подключение к Microsoft Search из внешнего источника.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 49e268f894b6733eb3f44d36fa34bc7c80df0ded
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498919"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="f098c-103">Тип ресурса Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="f098c-103">externalConnection resource type</span></span>

<span data-ttu-id="f098c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f098c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f098c-105">Подключение к Microsoft Search из внешнего источника.</span><span class="sxs-lookup"><span data-stu-id="f098c-105">A connection to Microsoft Search from an external source.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="f098c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f098c-106">Methods</span></span>

| <span data-ttu-id="f098c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f098c-107">Method</span></span>                                                           | <span data-ttu-id="f098c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f098c-108">Return Type</span></span>                                   | <span data-ttu-id="f098c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f098c-109">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="f098c-110">Создание Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="f098c-110">Create externalConnection</span></span>](../api/external-post-connections.md) | <span data-ttu-id="f098c-111">externalConnection</span><span class="sxs-lookup"><span data-stu-id="f098c-111">externalConnection</span></span>                            | <span data-ttu-id="f098c-112">Создание нового Екстерналконнектион путем публикации в коллекции Connections.</span><span class="sxs-lookup"><span data-stu-id="f098c-112">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="f098c-113">Список Екстерналконнектионс</span><span class="sxs-lookup"><span data-stu-id="f098c-113">List externalConnections</span></span>](../api/externalconnection-list.md)    | <span data-ttu-id="f098c-114">Коллекция Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="f098c-114">externalConnection collection</span></span>                 | <span data-ttu-id="f098c-115">Получение коллекции объектов Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="f098c-115">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="f098c-116">Получение Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="f098c-116">Get externalConnection</span></span>](../api/externalconnection-get.md)       | <span data-ttu-id="f098c-117">externalConnection</span><span class="sxs-lookup"><span data-stu-id="f098c-117">externalConnection</span></span>                            | <span data-ttu-id="f098c-118">Чтение свойств и связей объекта Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="f098c-118">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="f098c-119">Обновление Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="f098c-119">Update externalConnection</span></span>](../api/externalconnection-update.md) | <span data-ttu-id="f098c-120">externalConnection</span><span class="sxs-lookup"><span data-stu-id="f098c-120">externalConnection</span></span>                            | <span data-ttu-id="f098c-121">Обновление объекта Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="f098c-121">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="f098c-122">Удаление Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="f098c-122">Delete externalConnection</span></span>](../api/externalconnection-delete.md) | <span data-ttu-id="f098c-123">Нет</span><span class="sxs-lookup"><span data-stu-id="f098c-123">None</span></span>                                          | <span data-ttu-id="f098c-124">Удаление объекта Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="f098c-124">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="f098c-125">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="f098c-125">Create schema</span></span>](../api/externalconnection-post-schema.md)        | <span data-ttu-id="f098c-126">Нет *или* [схема](schema.md)</span><span class="sxs-lookup"><span data-stu-id="f098c-126">None *or* [schema](schema.md)</span></span>                 | <span data-ttu-id="f098c-127">Регистрация схемы подключения.</span><span class="sxs-lookup"><span data-stu-id="f098c-127">Register connection schema.</span></span> |
| [<span data-ttu-id="f098c-128">Получение операции</span><span class="sxs-lookup"><span data-stu-id="f098c-128">Get operation</span></span>](../api/connectionoperation-get.md)               | [<span data-ttu-id="f098c-129">коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="f098c-129">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="f098c-130">Получение состояния асинхронного запроса для создания схемы подключения.</span><span class="sxs-lookup"><span data-stu-id="f098c-130">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="f098c-131">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f098c-131">Create externalItem</span></span>](../api/externalconnection-put-items.md)    | [<span data-ttu-id="f098c-132">externalItem</span><span class="sxs-lookup"><span data-stu-id="f098c-132">externalItem</span></span>](externalitem.md)               | <span data-ttu-id="f098c-133">Создание нового Екстерналитем путем публикации в коллекции Items.</span><span class="sxs-lookup"><span data-stu-id="f098c-133">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="f098c-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="f098c-134">Properties</span></span>

| <span data-ttu-id="f098c-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="f098c-135">Property</span></span>      | <span data-ttu-id="f098c-136">Тип</span><span class="sxs-lookup"><span data-stu-id="f098c-136">Type</span></span>                              | <span data-ttu-id="f098c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="f098c-137">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="f098c-138">конфигурацион</span><span class="sxs-lookup"><span data-stu-id="f098c-138">configuration</span></span> | [<span data-ttu-id="f098c-139">configuration</span><span class="sxs-lookup"><span data-stu-id="f098c-139">configuration</span></span>](configuration.md) | <span data-ttu-id="f098c-140">Задает дополнительные идентификаторы приложений, которым разрешено управлять подключением и индексировать содержимое в подключении.</span><span class="sxs-lookup"><span data-stu-id="f098c-140">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="f098c-141">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="f098c-141">Optional.</span></span> |
| <span data-ttu-id="f098c-142">description</span><span class="sxs-lookup"><span data-stu-id="f098c-142">description</span></span>   | <span data-ttu-id="f098c-143">String</span><span class="sxs-lookup"><span data-stu-id="f098c-143">String</span></span>                            | <span data-ttu-id="f098c-144">Описание подключения, отображаемое в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f098c-144">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="f098c-145">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="f098c-145">Optional.</span></span> |
| <span data-ttu-id="f098c-146">id</span><span class="sxs-lookup"><span data-stu-id="f098c-146">id</span></span>            | <span data-ttu-id="f098c-147">Строка</span><span class="sxs-lookup"><span data-stu-id="f098c-147">String</span></span>                            | <span data-ttu-id="f098c-148">Предоставленный разработчиком уникальный идентификатор подключения в клиенте Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f098c-148">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="f098c-149">Максимальная длина 32 символов.</span><span class="sxs-lookup"><span data-stu-id="f098c-149">Maximum length of 32 characters.</span></span> <span data-ttu-id="f098c-150">Должно содержать только буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="f098c-150">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="f098c-151">`Microsoft` Не может начинаться с одного из следующих значений: `None`, `Directory`, `Exchange`, `ExchangeArchive` `LinkedIn` `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams`,,,,,,, `Yammer`,. `Connectors`</span><span class="sxs-lookup"><span data-stu-id="f098c-151">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`.</span></span> <span data-ttu-id="f098c-152">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="f098c-152">Required.</span></span> |
| <span data-ttu-id="f098c-153">name</span><span class="sxs-lookup"><span data-stu-id="f098c-153">name</span></span>          | <span data-ttu-id="f098c-154">String</span><span class="sxs-lookup"><span data-stu-id="f098c-154">String</span></span>                            | <span data-ttu-id="f098c-155">Отображаемое имя подключения, отображаемое в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f098c-155">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="f098c-156">Максимальная длина 128 символов.</span><span class="sxs-lookup"><span data-stu-id="f098c-156">Maximum length of 128 characters.</span></span> <span data-ttu-id="f098c-157">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="f098c-157">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f098c-158">Связи</span><span class="sxs-lookup"><span data-stu-id="f098c-158">Relationships</span></span>

| <span data-ttu-id="f098c-159">Связь</span><span class="sxs-lookup"><span data-stu-id="f098c-159">Relationship</span></span> | <span data-ttu-id="f098c-160">Тип</span><span class="sxs-lookup"><span data-stu-id="f098c-160">Type</span></span>                                                     | <span data-ttu-id="f098c-161">Описание</span><span class="sxs-lookup"><span data-stu-id="f098c-161">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="f098c-162">items</span><span class="sxs-lookup"><span data-stu-id="f098c-162">items</span></span>        | <span data-ttu-id="f098c-163">Коллекция [екстерналитем](externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="f098c-163">[externalItem](externalitem.md) collection</span></span>               | <span data-ttu-id="f098c-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f098c-p105">Read-only. Nullable.</span></span> |
| <span data-ttu-id="f098c-166">operations</span><span class="sxs-lookup"><span data-stu-id="f098c-166">operations</span></span>   | <span data-ttu-id="f098c-167">Коллекция [коннектионоператион](connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="f098c-167">[connectionOperation](connectionoperation.md) collection</span></span> | <span data-ttu-id="f098c-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f098c-168">Read-only.</span></span> <span data-ttu-id="f098c-169">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f098c-169">Nullable.</span></span> |
| <span data-ttu-id="f098c-170">схемы</span><span class="sxs-lookup"><span data-stu-id="f098c-170">schema</span></span>       | [<span data-ttu-id="f098c-171">schema</span><span class="sxs-lookup"><span data-stu-id="f098c-171">schema</span></span>](schema.md)                                      | <span data-ttu-id="f098c-p107">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f098c-p107">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f098c-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f098c-174">JSON representation</span></span>

<span data-ttu-id="f098c-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f098c-175">The following is a JSON representation of the resource.</span></span>

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
  "name": "String"
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
