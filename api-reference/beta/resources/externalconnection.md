---
title: Тип ресурса externalConnection
description: Подключение — это логический контейнер для внешнего контента в Microsoft Graph
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4355ffe51fe1b160c7fb486272e85f2b2cf0bf2c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161712"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="a4e8f-103">Тип ресурса externalConnection</span><span class="sxs-lookup"><span data-stu-id="a4e8f-103">externalConnection resource type</span></span>

<span data-ttu-id="a4e8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4e8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4e8f-105">Логический контейнер для добавления контента из внешнего источника в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-105">A logical container to add content from an external source into Microsoft Graph.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="a4e8f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a4e8f-106">Methods</span></span>

| <span data-ttu-id="a4e8f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a4e8f-107">Method</span></span>                                                           | <span data-ttu-id="a4e8f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a4e8f-108">Return Type</span></span>                                   | <span data-ttu-id="a4e8f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a4e8f-109">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="a4e8f-110">Создание externalConnection</span><span class="sxs-lookup"><span data-stu-id="a4e8f-110">Create externalConnection</span></span>](../api/external-post-connections.md) | <span data-ttu-id="a4e8f-111">externalConnection</span><span class="sxs-lookup"><span data-stu-id="a4e8f-111">externalConnection</span></span>                            | <span data-ttu-id="a4e8f-112">Создание внешнего подключения путем публикации в коллекции подключений.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-112">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="a4e8f-113">Список externalConnections</span><span class="sxs-lookup"><span data-stu-id="a4e8f-113">List externalConnections</span></span>](../api/externalconnection-list.md)    | <span data-ttu-id="a4e8f-114">коллекция externalConnection</span><span class="sxs-lookup"><span data-stu-id="a4e8f-114">externalConnection collection</span></span>                 | <span data-ttu-id="a4e8f-115">Получить коллекцию объектов externalConnection.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-115">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="a4e8f-116">Get externalConnection</span><span class="sxs-lookup"><span data-stu-id="a4e8f-116">Get externalConnection</span></span>](../api/externalconnection-get.md)       | <span data-ttu-id="a4e8f-117">externalConnection</span><span class="sxs-lookup"><span data-stu-id="a4e8f-117">externalConnection</span></span>                            | <span data-ttu-id="a4e8f-118">Чтение свойств и связей объекта externalConnection.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-118">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="a4e8f-119">Обновление externalConnection</span><span class="sxs-lookup"><span data-stu-id="a4e8f-119">Update externalConnection</span></span>](../api/externalconnection-update.md) | <span data-ttu-id="a4e8f-120">externalConnection</span><span class="sxs-lookup"><span data-stu-id="a4e8f-120">externalConnection</span></span>                            | <span data-ttu-id="a4e8f-121">Обновление объекта externalConnection.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-121">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="a4e8f-122">Удаление externalConnection</span><span class="sxs-lookup"><span data-stu-id="a4e8f-122">Delete externalConnection</span></span>](../api/externalconnection-delete.md) | <span data-ttu-id="a4e8f-123">Нет</span><span class="sxs-lookup"><span data-stu-id="a4e8f-123">None</span></span>                                          | <span data-ttu-id="a4e8f-124">Удаление объекта externalConnection.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-124">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="a4e8f-125">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="a4e8f-125">Create schema</span></span>](../api/externalconnection-post-schema.md)        | <span data-ttu-id="a4e8f-126">Нет *или* [схема](schema.md)</span><span class="sxs-lookup"><span data-stu-id="a4e8f-126">None *or* [schema](schema.md)</span></span>                 | <span data-ttu-id="a4e8f-127">Зарегистрируйте схему подключения.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-127">Register connection schema.</span></span> |
| [<span data-ttu-id="a4e8f-128">Получить операцию</span><span class="sxs-lookup"><span data-stu-id="a4e8f-128">Get operation</span></span>](../api/connectionoperation-get.md)               | [<span data-ttu-id="a4e8f-129">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="a4e8f-129">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="a4e8f-130">Получите состояние асинхронного запроса для создания схемы подключения.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-130">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="a4e8f-131">Создание externalItem</span><span class="sxs-lookup"><span data-stu-id="a4e8f-131">Create externalItem</span></span>](../api/externalconnection-put-items.md)    | [<span data-ttu-id="a4e8f-132">externalItem</span><span class="sxs-lookup"><span data-stu-id="a4e8f-132">externalItem</span></span>](externalitem.md)               | <span data-ttu-id="a4e8f-133">Создание внешнегоitem путем публикации в коллекции элементов.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-133">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="a4e8f-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4e8f-134">Properties</span></span>

| <span data-ttu-id="a4e8f-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4e8f-135">Property</span></span>      | <span data-ttu-id="a4e8f-136">Тип</span><span class="sxs-lookup"><span data-stu-id="a4e8f-136">Type</span></span>                              | <span data-ttu-id="a4e8f-137">Описание</span><span class="sxs-lookup"><span data-stu-id="a4e8f-137">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="a4e8f-138">configuration</span><span class="sxs-lookup"><span data-stu-id="a4e8f-138">configuration</span></span> | [<span data-ttu-id="a4e8f-139">configuration</span><span class="sxs-lookup"><span data-stu-id="a4e8f-139">configuration</span></span>](configuration.md) | <span data-ttu-id="a4e8f-140">Указывает дополнительные ИД приложений, которые разрешено использовать для управления подключением и индексации содержимого подключения.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-140">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="a4e8f-141">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-141">Optional.</span></span> |
| <span data-ttu-id="a4e8f-142">description</span><span class="sxs-lookup"><span data-stu-id="a4e8f-142">description</span></span>   | <span data-ttu-id="a4e8f-143">String</span><span class="sxs-lookup"><span data-stu-id="a4e8f-143">String</span></span>                            | <span data-ttu-id="a4e8f-144">Описание подключения, отображаемого в Центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-144">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="a4e8f-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-145">Optional.</span></span> |
| <span data-ttu-id="a4e8f-146">id</span><span class="sxs-lookup"><span data-stu-id="a4e8f-146">id</span></span>            | <span data-ttu-id="a4e8f-147">String</span><span class="sxs-lookup"><span data-stu-id="a4e8f-147">String</span></span>                            | <span data-ttu-id="a4e8f-148">Уникальный ИД подключения в клиенте Azure Active Directory, предоставленный разработчиком.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-148">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="a4e8f-149">Максимальная длина — 32 символа.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-149">Maximum length of 32 characters.</span></span> <span data-ttu-id="a4e8f-150">Должен содержать только буквы и цифры.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-150">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="a4e8f-151">Не может начинаться с одного из следующих `Microsoft` значений: `None` , , , , , , , , `Directory` , `Exchange` , `ExchangeArchive` `LinkedIn` `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` .</span><span class="sxs-lookup"><span data-stu-id="a4e8f-151">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`.</span></span> <span data-ttu-id="a4e8f-152">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-152">Required.</span></span> |
| <span data-ttu-id="a4e8f-153">name</span><span class="sxs-lookup"><span data-stu-id="a4e8f-153">name</span></span>          | <span data-ttu-id="a4e8f-154">String</span><span class="sxs-lookup"><span data-stu-id="a4e8f-154">String</span></span>                            | <span data-ttu-id="a4e8f-155">Отображаемого имени подключения, отображаемого в Центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-155">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="a4e8f-156">Максимальная длина — 128 символов.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-156">Maximum length of 128 characters.</span></span> <span data-ttu-id="a4e8f-157">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-157">Required.</span></span> |
| <span data-ttu-id="a4e8f-158">state</span><span class="sxs-lookup"><span data-stu-id="a4e8f-158">state</span></span>         | <span data-ttu-id="a4e8f-159">connectionState</span><span class="sxs-lookup"><span data-stu-id="a4e8f-159">connectionState</span></span>                   | <span data-ttu-id="a4e8f-160">Указывает текущее состояние подключения.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-160">Indicates the current state of the connection.</span></span> <span data-ttu-id="a4e8f-161">Возможные значения: `draft` `ready` , , и `obsolete` `limitExceeded` .</span><span class="sxs-lookup"><span data-stu-id="a4e8f-161">Possible values are `draft`, `ready`, `obsolete`, and `limitExceeded`.</span></span> <span data-ttu-id="a4e8f-162">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-162">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a4e8f-163">Связи</span><span class="sxs-lookup"><span data-stu-id="a4e8f-163">Relationships</span></span>

| <span data-ttu-id="a4e8f-164">Связь</span><span class="sxs-lookup"><span data-stu-id="a4e8f-164">Relationship</span></span> | <span data-ttu-id="a4e8f-165">Тип</span><span class="sxs-lookup"><span data-stu-id="a4e8f-165">Type</span></span>                                                     | <span data-ttu-id="a4e8f-166">Описание</span><span class="sxs-lookup"><span data-stu-id="a4e8f-166">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="a4e8f-167">items</span><span class="sxs-lookup"><span data-stu-id="a4e8f-167">items</span></span>        | <span data-ttu-id="a4e8f-168">[коллекция externalItem](externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="a4e8f-168">[externalItem](externalitem.md) collection</span></span>               | <span data-ttu-id="a4e8f-p106">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-p106">Read-only. Nullable.</span></span> |
| <span data-ttu-id="a4e8f-171">operations</span><span class="sxs-lookup"><span data-stu-id="a4e8f-171">operations</span></span>   | <span data-ttu-id="a4e8f-172">[Коллекция connectionOperation](connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="a4e8f-172">[connectionOperation](connectionoperation.md) collection</span></span> | <span data-ttu-id="a4e8f-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-173">Read-only.</span></span> <span data-ttu-id="a4e8f-174">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-174">Nullable.</span></span> |
| <span data-ttu-id="a4e8f-175">схема</span><span class="sxs-lookup"><span data-stu-id="a4e8f-175">schema</span></span>       | [<span data-ttu-id="a4e8f-176">schema</span><span class="sxs-lookup"><span data-stu-id="a4e8f-176">schema</span></span>](schema.md)                                      | <span data-ttu-id="a4e8f-p108">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-p108">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a4e8f-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4e8f-179">JSON representation</span></span>

<span data-ttu-id="a4e8f-180">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4e8f-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnection",
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
