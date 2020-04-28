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
# <a name="externalconnection-resource-type"></a><span data-ttu-id="4eb4e-103">Тип ресурса Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="4eb4e-103">externalConnection resource type</span></span>

<span data-ttu-id="4eb4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4eb4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4eb4e-105">Подключение к Microsoft Search из внешнего источника.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-105">A connection to Microsoft Search from an external source.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="4eb4e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4eb4e-106">Methods</span></span>

| <span data-ttu-id="4eb4e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4eb4e-107">Method</span></span>                                                           | <span data-ttu-id="4eb4e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4eb4e-108">Return Type</span></span>                                   | <span data-ttu-id="4eb4e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4eb4e-109">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="4eb4e-110">Создание Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="4eb4e-110">Create externalConnection</span></span>](../api/external-post-connections.md) | <span data-ttu-id="4eb4e-111">externalConnection</span><span class="sxs-lookup"><span data-stu-id="4eb4e-111">externalConnection</span></span>                            | <span data-ttu-id="4eb4e-112">Создание нового Екстерналконнектион путем публикации в коллекции Connections.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-112">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="4eb4e-113">Список Екстерналконнектионс</span><span class="sxs-lookup"><span data-stu-id="4eb4e-113">List externalConnections</span></span>](../api/externalconnection-list.md)    | <span data-ttu-id="4eb4e-114">Коллекция Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="4eb4e-114">externalConnection collection</span></span>                 | <span data-ttu-id="4eb4e-115">Получение коллекции объектов Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-115">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="4eb4e-116">Получение Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="4eb4e-116">Get externalConnection</span></span>](../api/externalconnection-get.md)       | <span data-ttu-id="4eb4e-117">externalConnection</span><span class="sxs-lookup"><span data-stu-id="4eb4e-117">externalConnection</span></span>                            | <span data-ttu-id="4eb4e-118">Чтение свойств и связей объекта Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-118">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="4eb4e-119">Обновление Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="4eb4e-119">Update externalConnection</span></span>](../api/externalconnection-update.md) | <span data-ttu-id="4eb4e-120">externalConnection</span><span class="sxs-lookup"><span data-stu-id="4eb4e-120">externalConnection</span></span>                            | <span data-ttu-id="4eb4e-121">Обновление объекта Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-121">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="4eb4e-122">Удаление Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="4eb4e-122">Delete externalConnection</span></span>](../api/externalconnection-delete.md) | <span data-ttu-id="4eb4e-123">Нет</span><span class="sxs-lookup"><span data-stu-id="4eb4e-123">None</span></span>                                          | <span data-ttu-id="4eb4e-124">Удаление объекта Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-124">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="4eb4e-125">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="4eb4e-125">Create schema</span></span>](../api/externalconnection-post-schema.md)        | <span data-ttu-id="4eb4e-126">Нет *или* [схема](schema.md)</span><span class="sxs-lookup"><span data-stu-id="4eb4e-126">None *or* [schema](schema.md)</span></span>                 | <span data-ttu-id="4eb4e-127">Регистрация схемы подключения.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-127">Register connection schema.</span></span> |
| [<span data-ttu-id="4eb4e-128">Получение операции</span><span class="sxs-lookup"><span data-stu-id="4eb4e-128">Get operation</span></span>](../api/connectionoperation-get.md)               | [<span data-ttu-id="4eb4e-129">коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="4eb4e-129">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="4eb4e-130">Получение состояния асинхронного запроса для создания схемы подключения.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-130">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="4eb4e-131">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="4eb4e-131">Create externalItem</span></span>](../api/externalconnection-put-items.md)    | [<span data-ttu-id="4eb4e-132">externalItem</span><span class="sxs-lookup"><span data-stu-id="4eb4e-132">externalItem</span></span>](externalitem.md)               | <span data-ttu-id="4eb4e-133">Создание нового Екстерналитем путем публикации в коллекции Items.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-133">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="4eb4e-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="4eb4e-134">Properties</span></span>

| <span data-ttu-id="4eb4e-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="4eb4e-135">Property</span></span>      | <span data-ttu-id="4eb4e-136">Тип</span><span class="sxs-lookup"><span data-stu-id="4eb4e-136">Type</span></span>                              | <span data-ttu-id="4eb4e-137">Описание</span><span class="sxs-lookup"><span data-stu-id="4eb4e-137">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="4eb4e-138">конфигурацион</span><span class="sxs-lookup"><span data-stu-id="4eb4e-138">configuration</span></span> | [<span data-ttu-id="4eb4e-139">configuration</span><span class="sxs-lookup"><span data-stu-id="4eb4e-139">configuration</span></span>](configuration.md) | <span data-ttu-id="4eb4e-140">Задает дополнительные идентификаторы приложений, которым разрешено управлять подключением и индексировать содержимое в подключении.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-140">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="4eb4e-141">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-141">Optional.</span></span> |
| <span data-ttu-id="4eb4e-142">description</span><span class="sxs-lookup"><span data-stu-id="4eb4e-142">description</span></span>   | <span data-ttu-id="4eb4e-143">String</span><span class="sxs-lookup"><span data-stu-id="4eb4e-143">String</span></span>                            | <span data-ttu-id="4eb4e-144">Описание подключения, отображаемое в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-144">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="4eb4e-145">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-145">Optional.</span></span> |
| <span data-ttu-id="4eb4e-146">id</span><span class="sxs-lookup"><span data-stu-id="4eb4e-146">id</span></span>            | <span data-ttu-id="4eb4e-147">Строка</span><span class="sxs-lookup"><span data-stu-id="4eb4e-147">String</span></span>                            | <span data-ttu-id="4eb4e-148">Предоставленный разработчиком уникальный идентификатор подключения в клиенте Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-148">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="4eb4e-149">Максимальная длина 32 символов.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-149">Maximum length of 32 characters.</span></span> <span data-ttu-id="4eb4e-150">Должно содержать только буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-150">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="4eb4e-151">`Microsoft` Не может начинаться с одного из следующих значений: `None`, `Directory`, `Exchange`, `ExchangeArchive` `LinkedIn` `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams`,,,,,,, `Yammer`,. `Connectors`</span><span class="sxs-lookup"><span data-stu-id="4eb4e-151">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`.</span></span> <span data-ttu-id="4eb4e-152">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-152">Required.</span></span> |
| <span data-ttu-id="4eb4e-153">name</span><span class="sxs-lookup"><span data-stu-id="4eb4e-153">name</span></span>          | <span data-ttu-id="4eb4e-154">String</span><span class="sxs-lookup"><span data-stu-id="4eb4e-154">String</span></span>                            | <span data-ttu-id="4eb4e-155">Отображаемое имя подключения, отображаемое в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-155">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="4eb4e-156">Максимальная длина 128 символов.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-156">Maximum length of 128 characters.</span></span> <span data-ttu-id="4eb4e-157">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-157">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4eb4e-158">Связи</span><span class="sxs-lookup"><span data-stu-id="4eb4e-158">Relationships</span></span>

| <span data-ttu-id="4eb4e-159">Связь</span><span class="sxs-lookup"><span data-stu-id="4eb4e-159">Relationship</span></span> | <span data-ttu-id="4eb4e-160">Тип</span><span class="sxs-lookup"><span data-stu-id="4eb4e-160">Type</span></span>                                                     | <span data-ttu-id="4eb4e-161">Описание</span><span class="sxs-lookup"><span data-stu-id="4eb4e-161">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="4eb4e-162">items</span><span class="sxs-lookup"><span data-stu-id="4eb4e-162">items</span></span>        | <span data-ttu-id="4eb4e-163">Коллекция [екстерналитем](externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="4eb4e-163">[externalItem](externalitem.md) collection</span></span>               | <span data-ttu-id="4eb4e-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-p105">Read-only. Nullable.</span></span> |
| <span data-ttu-id="4eb4e-166">operations</span><span class="sxs-lookup"><span data-stu-id="4eb4e-166">operations</span></span>   | <span data-ttu-id="4eb4e-167">Коллекция [коннектионоператион](connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="4eb4e-167">[connectionOperation](connectionoperation.md) collection</span></span> | <span data-ttu-id="4eb4e-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-168">Read-only.</span></span> <span data-ttu-id="4eb4e-169">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-169">Nullable.</span></span> |
| <span data-ttu-id="4eb4e-170">схемы</span><span class="sxs-lookup"><span data-stu-id="4eb4e-170">schema</span></span>       | [<span data-ttu-id="4eb4e-171">schema</span><span class="sxs-lookup"><span data-stu-id="4eb4e-171">schema</span></span>](schema.md)                                      | <span data-ttu-id="4eb4e-p107">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-p107">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4eb4e-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4eb4e-174">JSON representation</span></span>

<span data-ttu-id="4eb4e-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-175">The following is a JSON representation of the resource.</span></span>

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
