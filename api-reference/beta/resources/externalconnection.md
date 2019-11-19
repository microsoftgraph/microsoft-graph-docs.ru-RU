---
title: Тип ресурса Екстерналконнектион
description: Подключение к Microsoft Search из внешнего источника.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 78752e2fe3375c10dcce57e3ba23e890b0ab66b5
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704180"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="158cb-103">Тип ресурса Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="158cb-103">externalConnection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="158cb-104">Подключение к Microsoft Search из внешнего источника.</span><span class="sxs-lookup"><span data-stu-id="158cb-104">A connection to Microsoft Search from an external source.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="158cb-105">Методы</span><span class="sxs-lookup"><span data-stu-id="158cb-105">Methods</span></span>

| <span data-ttu-id="158cb-106">Метод</span><span class="sxs-lookup"><span data-stu-id="158cb-106">Method</span></span>                                                           | <span data-ttu-id="158cb-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="158cb-107">Return Type</span></span>                                   | <span data-ttu-id="158cb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="158cb-108">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="158cb-109">Создание Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="158cb-109">Create externalConnection</span></span>](../api/external-post-connections.md) | <span data-ttu-id="158cb-110">externalConnection</span><span class="sxs-lookup"><span data-stu-id="158cb-110">externalConnection</span></span>                            | <span data-ttu-id="158cb-111">Создание нового Екстерналконнектион путем публикации в коллекции Connections.</span><span class="sxs-lookup"><span data-stu-id="158cb-111">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="158cb-112">Список Екстерналконнектионс</span><span class="sxs-lookup"><span data-stu-id="158cb-112">List externalConnections</span></span>](../api/externalconnection-list.md)    | <span data-ttu-id="158cb-113">Коллекция Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="158cb-113">externalConnection collection</span></span>                 | <span data-ttu-id="158cb-114">Получение коллекции объектов Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="158cb-114">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="158cb-115">Получение Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="158cb-115">Get externalConnection</span></span>](../api/externalconnection-get.md)       | <span data-ttu-id="158cb-116">externalConnection</span><span class="sxs-lookup"><span data-stu-id="158cb-116">externalConnection</span></span>                            | <span data-ttu-id="158cb-117">Чтение свойств и связей объекта Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="158cb-117">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="158cb-118">Обновление Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="158cb-118">Update externalConnection</span></span>](../api/externalconnection-update.md) | <span data-ttu-id="158cb-119">externalConnection</span><span class="sxs-lookup"><span data-stu-id="158cb-119">externalConnection</span></span>                            | <span data-ttu-id="158cb-120">Обновление объекта Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="158cb-120">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="158cb-121">Удаление Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="158cb-121">Delete externalConnection</span></span>](../api/externalconnection-delete.md) | <span data-ttu-id="158cb-122">Нет</span><span class="sxs-lookup"><span data-stu-id="158cb-122">None</span></span>                                          | <span data-ttu-id="158cb-123">Удаление объекта Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="158cb-123">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="158cb-124">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="158cb-124">Create schema</span></span>](../api/externalconnection-post-schema.md)        | <span data-ttu-id="158cb-125">Нет *или* [схема](schema.md)</span><span class="sxs-lookup"><span data-stu-id="158cb-125">None *or* [schema](schema.md)</span></span>                 | <span data-ttu-id="158cb-126">Регистрация схемы подключения.</span><span class="sxs-lookup"><span data-stu-id="158cb-126">Register connection schema.</span></span> |
| [<span data-ttu-id="158cb-127">Получение операции</span><span class="sxs-lookup"><span data-stu-id="158cb-127">Get operation</span></span>](../api/connectionoperation-get.md)               | [<span data-ttu-id="158cb-128">коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="158cb-128">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="158cb-129">Получение состояния асинхронного запроса для создания схемы подключения.</span><span class="sxs-lookup"><span data-stu-id="158cb-129">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="158cb-130">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="158cb-130">Create externalItem</span></span>](../api/externalconnection-put-items.md)    | [<span data-ttu-id="158cb-131">externalItem</span><span class="sxs-lookup"><span data-stu-id="158cb-131">externalItem</span></span>](externalitem.md)               | <span data-ttu-id="158cb-132">Создание нового Екстерналитем путем публикации в коллекции Items.</span><span class="sxs-lookup"><span data-stu-id="158cb-132">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="158cb-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="158cb-133">Properties</span></span>

| <span data-ttu-id="158cb-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="158cb-134">Property</span></span>      | <span data-ttu-id="158cb-135">Тип</span><span class="sxs-lookup"><span data-stu-id="158cb-135">Type</span></span>                              | <span data-ttu-id="158cb-136">Описание</span><span class="sxs-lookup"><span data-stu-id="158cb-136">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="158cb-137">конфигурацион</span><span class="sxs-lookup"><span data-stu-id="158cb-137">configuration</span></span> | [<span data-ttu-id="158cb-138">configuration</span><span class="sxs-lookup"><span data-stu-id="158cb-138">configuration</span></span>](configuration.md) | <span data-ttu-id="158cb-139">Задает дополнительные идентификаторы приложений, которым разрешено управлять подключением и индексировать содержимое в подключении.</span><span class="sxs-lookup"><span data-stu-id="158cb-139">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="158cb-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="158cb-140">Optional.</span></span> |
| <span data-ttu-id="158cb-141">description</span><span class="sxs-lookup"><span data-stu-id="158cb-141">description</span></span>   | <span data-ttu-id="158cb-142">String</span><span class="sxs-lookup"><span data-stu-id="158cb-142">String</span></span>                            | <span data-ttu-id="158cb-143">Описание подключения, отображаемое в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="158cb-143">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="158cb-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="158cb-144">Optional.</span></span> |
| <span data-ttu-id="158cb-145">id</span><span class="sxs-lookup"><span data-stu-id="158cb-145">id</span></span>            | <span data-ttu-id="158cb-146">Строка</span><span class="sxs-lookup"><span data-stu-id="158cb-146">String</span></span>                            | <span data-ttu-id="158cb-147">Предоставленный разработчиком уникальный идентификатор подключения в клиенте Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="158cb-147">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="158cb-148">Максимальная длина 32 символов.</span><span class="sxs-lookup"><span data-stu-id="158cb-148">Maximum length of 32 characters.</span></span> <span data-ttu-id="158cb-149">Должно содержать только буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="158cb-149">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="158cb-150">`Microsoft` Не может начинаться с одного из следующих значений: `None`, `Directory`, `Exchange`, `ExchangeArchive` `LinkedIn` `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams`,,,,,,, `Yammer`,. `Connectors`</span><span class="sxs-lookup"><span data-stu-id="158cb-150">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`.</span></span> <span data-ttu-id="158cb-151">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="158cb-151">Required.</span></span> |
| <span data-ttu-id="158cb-152">name</span><span class="sxs-lookup"><span data-stu-id="158cb-152">name</span></span>          | <span data-ttu-id="158cb-153">String</span><span class="sxs-lookup"><span data-stu-id="158cb-153">String</span></span>                            | <span data-ttu-id="158cb-154">Отображаемое имя подключения, отображаемое в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="158cb-154">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="158cb-155">Максимальная длина 128 символов.</span><span class="sxs-lookup"><span data-stu-id="158cb-155">Maximum length of 128 characters.</span></span> <span data-ttu-id="158cb-156">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="158cb-156">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="158cb-157">Связи</span><span class="sxs-lookup"><span data-stu-id="158cb-157">Relationships</span></span>

| <span data-ttu-id="158cb-158">Связь</span><span class="sxs-lookup"><span data-stu-id="158cb-158">Relationship</span></span> | <span data-ttu-id="158cb-159">Тип</span><span class="sxs-lookup"><span data-stu-id="158cb-159">Type</span></span>                                                     | <span data-ttu-id="158cb-160">Описание</span><span class="sxs-lookup"><span data-stu-id="158cb-160">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="158cb-161">items</span><span class="sxs-lookup"><span data-stu-id="158cb-161">items</span></span>        | <span data-ttu-id="158cb-162">Коллекция [екстерналитем](externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="158cb-162">[externalItem](externalitem.md) collection</span></span>               | <span data-ttu-id="158cb-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="158cb-p105">Read-only. Nullable.</span></span> |
| <span data-ttu-id="158cb-165">operations</span><span class="sxs-lookup"><span data-stu-id="158cb-165">operations</span></span>   | <span data-ttu-id="158cb-166">Коллекция [коннектионоператион](connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="158cb-166">[connectionOperation](connectionoperation.md) collection</span></span> | <span data-ttu-id="158cb-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="158cb-167">Read-only.</span></span> <span data-ttu-id="158cb-168">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="158cb-168">Nullable.</span></span> |
| <span data-ttu-id="158cb-169">схемы</span><span class="sxs-lookup"><span data-stu-id="158cb-169">schema</span></span>       | [<span data-ttu-id="158cb-170">schema</span><span class="sxs-lookup"><span data-stu-id="158cb-170">schema</span></span>](schema.md)                                      | <span data-ttu-id="158cb-p107">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="158cb-p107">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="158cb-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="158cb-173">JSON representation</span></span>

<span data-ttu-id="158cb-174">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="158cb-174">The following is a JSON representation of the resource.</span></span>

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
