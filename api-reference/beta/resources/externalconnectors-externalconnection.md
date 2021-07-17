---
title: тип ресурса externalConnection
description: Подключение является логическим контейнером для внешнего контента в Microsoft Graph
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 76fa391d1ce9937bc1799e9bc4ae9470c0794497
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467824"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="4bb47-103">тип ресурса externalConnection</span><span class="sxs-lookup"><span data-stu-id="4bb47-103">externalConnection resource type</span></span>

<span data-ttu-id="4bb47-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="4bb47-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bb47-105">Логический контейнер для добавления контента из внешнего источника в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4bb47-105">A logical container to add content from an external source into Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="4bb47-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4bb47-106">Methods</span></span>

| <span data-ttu-id="4bb47-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4bb47-107">Method</span></span>                                                           | <span data-ttu-id="4bb47-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4bb47-108">Return Type</span></span>                                   | <span data-ttu-id="4bb47-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4bb47-109">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="4bb47-110">Создание externalConnection</span><span class="sxs-lookup"><span data-stu-id="4bb47-110">Create externalConnection</span></span>](../api/externalconnectors-external-post-connections.md) | <span data-ttu-id="4bb47-111">externalConnection</span><span class="sxs-lookup"><span data-stu-id="4bb47-111">externalConnection</span></span>                            | <span data-ttu-id="4bb47-112">Создайте новую externalConnection, разместив в коллекции подключений.</span><span class="sxs-lookup"><span data-stu-id="4bb47-112">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="4bb47-113">Список externalConnections</span><span class="sxs-lookup"><span data-stu-id="4bb47-113">List externalConnections</span></span>](../api/externalconnectors-externalconnection-list.md)    | <span data-ttu-id="4bb47-114">коллекция externalConnection</span><span class="sxs-lookup"><span data-stu-id="4bb47-114">externalConnection collection</span></span>                 | <span data-ttu-id="4bb47-115">Получите коллекцию объектов externalConnection.</span><span class="sxs-lookup"><span data-stu-id="4bb47-115">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="4bb47-116">Get externalConnection</span><span class="sxs-lookup"><span data-stu-id="4bb47-116">Get externalConnection</span></span>](../api/externalconnectors-externalconnection-get.md)       | <span data-ttu-id="4bb47-117">externalConnection</span><span class="sxs-lookup"><span data-stu-id="4bb47-117">externalConnection</span></span>                            | <span data-ttu-id="4bb47-118">Чтение свойств и связей объекта externalConnection.</span><span class="sxs-lookup"><span data-stu-id="4bb47-118">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="4bb47-119">Обновление externalConnection</span><span class="sxs-lookup"><span data-stu-id="4bb47-119">Update externalConnection</span></span>](../api/externalconnectors-externalconnection-update.md) | <span data-ttu-id="4bb47-120">externalConnection</span><span class="sxs-lookup"><span data-stu-id="4bb47-120">externalConnection</span></span>                            | <span data-ttu-id="4bb47-121">Обновление объекта externalConnection.</span><span class="sxs-lookup"><span data-stu-id="4bb47-121">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="4bb47-122">Удаление externalConnection</span><span class="sxs-lookup"><span data-stu-id="4bb47-122">Delete externalConnection</span></span>](../api/externalconnectors-externalconnection-delete.md) | <span data-ttu-id="4bb47-123">Нет</span><span class="sxs-lookup"><span data-stu-id="4bb47-123">None</span></span>                                          | <span data-ttu-id="4bb47-124">Удаление объекта externalConnection.</span><span class="sxs-lookup"><span data-stu-id="4bb47-124">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="4bb47-125">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="4bb47-125">Create schema</span></span>](../api/externalconnectors-externalconnection-post-schema.md)        | <span data-ttu-id="4bb47-126">Нет *или* [схемы](externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="4bb47-126">None *or* [schema](externalconnectors-schema.md)</span></span>                 | <span data-ttu-id="4bb47-127">Схема подключения для регистрации.</span><span class="sxs-lookup"><span data-stu-id="4bb47-127">Register connection schema.</span></span> |
| [<span data-ttu-id="4bb47-128">Получить операцию</span><span class="sxs-lookup"><span data-stu-id="4bb47-128">Get operation</span></span>](../api/externalconnectors-connectionoperation-get.md)               | [<span data-ttu-id="4bb47-129">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="4bb47-129">connectionOperation</span></span>](externalconnectors-connectionoperation.md) | <span data-ttu-id="4bb47-130">Получите состояние асинхронного запроса для создания схемы подключения.</span><span class="sxs-lookup"><span data-stu-id="4bb47-130">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="4bb47-131">Создание externalItem</span><span class="sxs-lookup"><span data-stu-id="4bb47-131">Create externalItem</span></span>](../api/externalconnectors-externalconnection-put-items.md)    | [<span data-ttu-id="4bb47-132">externalItem</span><span class="sxs-lookup"><span data-stu-id="4bb47-132">externalItem</span></span>](externalconnectors-externalitem.md)               | <span data-ttu-id="4bb47-133">Создайте новый externalItem, разместив в коллекции элементов.</span><span class="sxs-lookup"><span data-stu-id="4bb47-133">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="4bb47-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="4bb47-134">Properties</span></span>

| <span data-ttu-id="4bb47-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bb47-135">Property</span></span>      | <span data-ttu-id="4bb47-136">Тип</span><span class="sxs-lookup"><span data-stu-id="4bb47-136">Type</span></span>                              | <span data-ttu-id="4bb47-137">Описание</span><span class="sxs-lookup"><span data-stu-id="4bb47-137">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="4bb47-138">configuration</span><span class="sxs-lookup"><span data-stu-id="4bb47-138">configuration</span></span> | [<span data-ttu-id="4bb47-139">microsoft.graph.externalConnectors.configuration</span><span class="sxs-lookup"><span data-stu-id="4bb47-139">microsoft.graph.externalConnectors.configuration</span></span>](externalconnectors-configuration.md) | <span data-ttu-id="4bb47-140">Указывает дополнительные ID-адреса приложений, которые разрешены для управления подключением и индексации контента в подключении.</span><span class="sxs-lookup"><span data-stu-id="4bb47-140">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="4bb47-141">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="4bb47-141">Optional.</span></span> |
| <span data-ttu-id="4bb47-142">description</span><span class="sxs-lookup"><span data-stu-id="4bb47-142">description</span></span>   | <span data-ttu-id="4bb47-143">String</span><span class="sxs-lookup"><span data-stu-id="4bb47-143">String</span></span>                            | <span data-ttu-id="4bb47-144">Описание подключения, отображаемого в Центр администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4bb47-144">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="4bb47-145">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="4bb47-145">Optional.</span></span> |
| <span data-ttu-id="4bb47-146">id</span><span class="sxs-lookup"><span data-stu-id="4bb47-146">id</span></span>            | <span data-ttu-id="4bb47-147">String</span><span class="sxs-lookup"><span data-stu-id="4bb47-147">String</span></span>                            | <span data-ttu-id="4bb47-148">Уникальный ID подключения, предоставленный разработчиком в Azure Active Directory клиента.</span><span class="sxs-lookup"><span data-stu-id="4bb47-148">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="4bb47-149">Длина должна быть от 3 до 32 символов.</span><span class="sxs-lookup"><span data-stu-id="4bb47-149">Must be between 3 and 32 characters in length.</span></span> <span data-ttu-id="4bb47-150">Должны содержаться только буквамерные символы.</span><span class="sxs-lookup"><span data-stu-id="4bb47-150">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="4bb47-151">Не может `Microsoft` начаться или быть одним из следующих значений: `None` , , , , , `Directory` `Exchange` `ExchangeArchive` `LinkedIn` `Mailbox` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` `TaskFabric` `PowerBI` `Assistant` `TopicEngine` `MSFT_All_Connectors` .</span><span class="sxs-lookup"><span data-stu-id="4bb47-151">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`, `TaskFabric`, `PowerBI`, `Assistant`, `TopicEngine`, `MSFT_All_Connectors`.</span></span> <span data-ttu-id="4bb47-152">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="4bb47-152">Required.</span></span> |
| <span data-ttu-id="4bb47-153">name</span><span class="sxs-lookup"><span data-stu-id="4bb47-153">name</span></span>          | <span data-ttu-id="4bb47-154">String</span><span class="sxs-lookup"><span data-stu-id="4bb47-154">String</span></span>                            | <span data-ttu-id="4bb47-155">Отображает имя подключения, отображаемого в Центр администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4bb47-155">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="4bb47-156">Максимальная длина 128 символов.</span><span class="sxs-lookup"><span data-stu-id="4bb47-156">Maximum length of 128 characters.</span></span> <span data-ttu-id="4bb47-157">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="4bb47-157">Required.</span></span> |
| <span data-ttu-id="4bb47-158">state</span><span class="sxs-lookup"><span data-stu-id="4bb47-158">state</span></span>         | <span data-ttu-id="4bb47-159">microsoft.graph.externalConnectors.connectionState</span><span class="sxs-lookup"><span data-stu-id="4bb47-159">microsoft.graph.externalConnectors.connectionState</span></span>                   | <span data-ttu-id="4bb47-160">Указывает текущее состояние подключения.</span><span class="sxs-lookup"><span data-stu-id="4bb47-160">Indicates the current state of the connection.</span></span> <span data-ttu-id="4bb47-161">Возможные значения `draft` , `ready` и `obsolete` `limitExceeded` .</span><span class="sxs-lookup"><span data-stu-id="4bb47-161">Possible values are `draft`, `ready`, `obsolete`, and `limitExceeded`.</span></span> <span data-ttu-id="4bb47-162">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bb47-162">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4bb47-163">Связи</span><span class="sxs-lookup"><span data-stu-id="4bb47-163">Relationships</span></span>

| <span data-ttu-id="4bb47-164">Связь</span><span class="sxs-lookup"><span data-stu-id="4bb47-164">Relationship</span></span> | <span data-ttu-id="4bb47-165">Тип</span><span class="sxs-lookup"><span data-stu-id="4bb47-165">Type</span></span>                                                     | <span data-ttu-id="4bb47-166">Описание</span><span class="sxs-lookup"><span data-stu-id="4bb47-166">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="4bb47-167">items</span><span class="sxs-lookup"><span data-stu-id="4bb47-167">items</span></span>        | <span data-ttu-id="4bb47-168">[коллекция microsoft.graph.externalConnectors.externalItem](externalconnectors-externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="4bb47-168">[microsoft.graph.externalConnectors.externalItem](externalconnectors-externalitem.md) collection</span></span>               | <span data-ttu-id="4bb47-p106">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4bb47-p106">Read-only. Nullable.</span></span> |
| <span data-ttu-id="4bb47-171">operations</span><span class="sxs-lookup"><span data-stu-id="4bb47-171">operations</span></span>   | <span data-ttu-id="4bb47-172">[коллекция microsoft.graph.externalConnectors.connectionOperation](externalconnectors-connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="4bb47-172">[microsoft.graph.externalConnectors.connectionOperation](externalconnectors-connectionoperation.md) collection</span></span> | <span data-ttu-id="4bb47-p107">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4bb47-p107">Read-only. Nullable.</span></span> |
| <span data-ttu-id="4bb47-175">schema</span><span class="sxs-lookup"><span data-stu-id="4bb47-175">schema</span></span>       | [<span data-ttu-id="4bb47-176">microsoft.graph.externalConnectors.schema</span><span class="sxs-lookup"><span data-stu-id="4bb47-176">microsoft.graph.externalConnectors.schema</span></span>](externalconnectors-schema.md)                                      | <span data-ttu-id="4bb47-p108">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4bb47-p108">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4bb47-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4bb47-179">JSON representation</span></span>

<span data-ttu-id="4bb47-180">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4bb47-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection",
  "keyProperty": "id"
}-->

```json
{
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
