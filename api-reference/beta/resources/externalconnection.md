---
title: тип ресурса externalConnection
description: Подключение является логическим контейнером для внешнего контента в Microsoft Graph
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4b0c0a56fc415c4f2f75ec4972909e31fc9bea14
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366571"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="027d5-103">тип ресурса externalConnection</span><span class="sxs-lookup"><span data-stu-id="027d5-103">externalConnection resource type</span></span>

<span data-ttu-id="027d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="027d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="027d5-105">Логический контейнер для добавления контента из внешнего источника в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="027d5-105">A logical container to add content from an external source into Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="027d5-106">Методы</span><span class="sxs-lookup"><span data-stu-id="027d5-106">Methods</span></span>

| <span data-ttu-id="027d5-107">Метод</span><span class="sxs-lookup"><span data-stu-id="027d5-107">Method</span></span>                                                           | <span data-ttu-id="027d5-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="027d5-108">Return Type</span></span>                                   | <span data-ttu-id="027d5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="027d5-109">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="027d5-110">Создание externalConnection</span><span class="sxs-lookup"><span data-stu-id="027d5-110">Create externalConnection</span></span>](../api/external-post-connections.md) | <span data-ttu-id="027d5-111">externalConnection</span><span class="sxs-lookup"><span data-stu-id="027d5-111">externalConnection</span></span>                            | <span data-ttu-id="027d5-112">Создайте новую externalConnection, разместив в коллекции подключений.</span><span class="sxs-lookup"><span data-stu-id="027d5-112">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="027d5-113">Список externalConnections</span><span class="sxs-lookup"><span data-stu-id="027d5-113">List externalConnections</span></span>](../api/externalconnection-list.md)    | <span data-ttu-id="027d5-114">коллекция externalConnection</span><span class="sxs-lookup"><span data-stu-id="027d5-114">externalConnection collection</span></span>                 | <span data-ttu-id="027d5-115">Получите коллекцию объектов externalConnection.</span><span class="sxs-lookup"><span data-stu-id="027d5-115">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="027d5-116">Get externalConnection</span><span class="sxs-lookup"><span data-stu-id="027d5-116">Get externalConnection</span></span>](../api/externalconnection-get.md)       | <span data-ttu-id="027d5-117">externalConnection</span><span class="sxs-lookup"><span data-stu-id="027d5-117">externalConnection</span></span>                            | <span data-ttu-id="027d5-118">Чтение свойств и связей объекта externalConnection.</span><span class="sxs-lookup"><span data-stu-id="027d5-118">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="027d5-119">Обновление externalConnection</span><span class="sxs-lookup"><span data-stu-id="027d5-119">Update externalConnection</span></span>](../api/externalconnection-update.md) | <span data-ttu-id="027d5-120">externalConnection</span><span class="sxs-lookup"><span data-stu-id="027d5-120">externalConnection</span></span>                            | <span data-ttu-id="027d5-121">Обновление объекта externalConnection.</span><span class="sxs-lookup"><span data-stu-id="027d5-121">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="027d5-122">Удаление externalConnection</span><span class="sxs-lookup"><span data-stu-id="027d5-122">Delete externalConnection</span></span>](../api/externalconnection-delete.md) | <span data-ttu-id="027d5-123">Нет</span><span class="sxs-lookup"><span data-stu-id="027d5-123">None</span></span>                                          | <span data-ttu-id="027d5-124">Удаление объекта externalConnection.</span><span class="sxs-lookup"><span data-stu-id="027d5-124">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="027d5-125">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="027d5-125">Create schema</span></span>](../api/externalconnection-post-schema.md)        | <span data-ttu-id="027d5-126">Нет *или* [схемы](schema.md)</span><span class="sxs-lookup"><span data-stu-id="027d5-126">None *or* [schema](schema.md)</span></span>                 | <span data-ttu-id="027d5-127">Схема подключения для регистрации.</span><span class="sxs-lookup"><span data-stu-id="027d5-127">Register connection schema.</span></span> |
| [<span data-ttu-id="027d5-128">Получить операцию</span><span class="sxs-lookup"><span data-stu-id="027d5-128">Get operation</span></span>](../api/connectionoperation-get.md)               | [<span data-ttu-id="027d5-129">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="027d5-129">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="027d5-130">Получите состояние асинхронного запроса для создания схемы подключения.</span><span class="sxs-lookup"><span data-stu-id="027d5-130">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="027d5-131">Создание externalItem</span><span class="sxs-lookup"><span data-stu-id="027d5-131">Create externalItem</span></span>](../api/externalconnection-put-items.md)    | [<span data-ttu-id="027d5-132">externalItem</span><span class="sxs-lookup"><span data-stu-id="027d5-132">externalItem</span></span>](externalitem.md)               | <span data-ttu-id="027d5-133">Создайте новый externalItem, разместив в коллекции элементов.</span><span class="sxs-lookup"><span data-stu-id="027d5-133">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="027d5-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="027d5-134">Properties</span></span>

| <span data-ttu-id="027d5-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="027d5-135">Property</span></span>      | <span data-ttu-id="027d5-136">Тип</span><span class="sxs-lookup"><span data-stu-id="027d5-136">Type</span></span>                              | <span data-ttu-id="027d5-137">Описание</span><span class="sxs-lookup"><span data-stu-id="027d5-137">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="027d5-138">configuration</span><span class="sxs-lookup"><span data-stu-id="027d5-138">configuration</span></span> | [<span data-ttu-id="027d5-139">configuration</span><span class="sxs-lookup"><span data-stu-id="027d5-139">configuration</span></span>](configuration.md) | <span data-ttu-id="027d5-140">Указывает дополнительные ID-адреса приложений, которые разрешены для управления подключением и индексации контента в подключении.</span><span class="sxs-lookup"><span data-stu-id="027d5-140">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="027d5-141">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="027d5-141">Optional.</span></span> |
| <span data-ttu-id="027d5-142">description</span><span class="sxs-lookup"><span data-stu-id="027d5-142">description</span></span>   | <span data-ttu-id="027d5-143">String</span><span class="sxs-lookup"><span data-stu-id="027d5-143">String</span></span>                            | <span data-ttu-id="027d5-144">Описание подключения, отображаемого в Центр администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="027d5-144">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="027d5-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="027d5-145">Optional.</span></span> |
| <span data-ttu-id="027d5-146">id</span><span class="sxs-lookup"><span data-stu-id="027d5-146">id</span></span>            | <span data-ttu-id="027d5-147">String</span><span class="sxs-lookup"><span data-stu-id="027d5-147">String</span></span>                            | <span data-ttu-id="027d5-148">Уникальный ID подключения, предоставленный разработчиком в Azure Active Directory клиента.</span><span class="sxs-lookup"><span data-stu-id="027d5-148">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="027d5-149">Максимальная длина — 32 символа.</span><span class="sxs-lookup"><span data-stu-id="027d5-149">Maximum length of 32 characters.</span></span> <span data-ttu-id="027d5-150">Должны содержаться только буквамерные символы.</span><span class="sxs-lookup"><span data-stu-id="027d5-150">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="027d5-151">Не может начаться с или быть `Microsoft` одним из следующих значений: `None` , , , , , , `Directory` `Exchange` `ExchangeArchive` `LinkedIn` `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` .</span><span class="sxs-lookup"><span data-stu-id="027d5-151">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`.</span></span> <span data-ttu-id="027d5-152">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="027d5-152">Required.</span></span> |
| <span data-ttu-id="027d5-153">name</span><span class="sxs-lookup"><span data-stu-id="027d5-153">name</span></span>          | <span data-ttu-id="027d5-154">String</span><span class="sxs-lookup"><span data-stu-id="027d5-154">String</span></span>                            | <span data-ttu-id="027d5-155">Отображает имя подключения, отображаемого в Центр администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="027d5-155">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="027d5-156">Максимальная длина 128 символов.</span><span class="sxs-lookup"><span data-stu-id="027d5-156">Maximum length of 128 characters.</span></span> <span data-ttu-id="027d5-157">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="027d5-157">Required.</span></span> |
| <span data-ttu-id="027d5-158">state</span><span class="sxs-lookup"><span data-stu-id="027d5-158">state</span></span>         | <span data-ttu-id="027d5-159">connectionState</span><span class="sxs-lookup"><span data-stu-id="027d5-159">connectionState</span></span>                   | <span data-ttu-id="027d5-160">Указывает текущее состояние подключения.</span><span class="sxs-lookup"><span data-stu-id="027d5-160">Indicates the current state of the connection.</span></span> <span data-ttu-id="027d5-161">Возможные значения `draft` , `ready` и `obsolete` `limitExceeded` .</span><span class="sxs-lookup"><span data-stu-id="027d5-161">Possible values are `draft`, `ready`, `obsolete`, and `limitExceeded`.</span></span> <span data-ttu-id="027d5-162">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="027d5-162">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="027d5-163">Связи</span><span class="sxs-lookup"><span data-stu-id="027d5-163">Relationships</span></span>

| <span data-ttu-id="027d5-164">Связь</span><span class="sxs-lookup"><span data-stu-id="027d5-164">Relationship</span></span> | <span data-ttu-id="027d5-165">Тип</span><span class="sxs-lookup"><span data-stu-id="027d5-165">Type</span></span>                                                     | <span data-ttu-id="027d5-166">Описание</span><span class="sxs-lookup"><span data-stu-id="027d5-166">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="027d5-167">items</span><span class="sxs-lookup"><span data-stu-id="027d5-167">items</span></span>        | <span data-ttu-id="027d5-168">[коллекция externalItem](externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="027d5-168">[externalItem](externalitem.md) collection</span></span>               | <span data-ttu-id="027d5-p106">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="027d5-p106">Read-only. Nullable.</span></span> |
| <span data-ttu-id="027d5-171">operations</span><span class="sxs-lookup"><span data-stu-id="027d5-171">operations</span></span>   | <span data-ttu-id="027d5-172">[коллекция connectionOperation](connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="027d5-172">[connectionOperation](connectionoperation.md) collection</span></span> | <span data-ttu-id="027d5-p107">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="027d5-p107">Read-only. Nullable.</span></span> |
| <span data-ttu-id="027d5-175">схема</span><span class="sxs-lookup"><span data-stu-id="027d5-175">schema</span></span>       | [<span data-ttu-id="027d5-176">schema</span><span class="sxs-lookup"><span data-stu-id="027d5-176">schema</span></span>](schema.md)                                      | <span data-ttu-id="027d5-p108">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="027d5-p108">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="027d5-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="027d5-179">JSON representation</span></span>

<span data-ttu-id="027d5-180">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="027d5-180">The following is a JSON representation of the resource.</span></span>

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
