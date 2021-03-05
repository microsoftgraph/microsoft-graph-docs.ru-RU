---
title: тип ресурса applicationTemplate
description: Представляет приложение в галерее приложений Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: dff7319444179dbe66698fa47691369ef3901340
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50476452"
---
# <a name="applicationtemplate-resource-type"></a><span data-ttu-id="cd6b4-103">тип ресурса applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="cd6b4-103">applicationTemplate resource type</span></span>

<span data-ttu-id="cd6b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd6b4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd6b4-105">Представляет приложение в галерее [приложений Azure AD.](/azure/active-directory/saas-apps/tutorial-list)</span><span class="sxs-lookup"><span data-stu-id="cd6b4-105">Represents an application in the [Azure AD application gallery](/azure/active-directory/saas-apps/tutorial-list).</span></span>

## <a name="methods"></a><span data-ttu-id="cd6b4-106">Методы</span><span class="sxs-lookup"><span data-stu-id="cd6b4-106">Methods</span></span>

| <span data-ttu-id="cd6b4-107">Метод</span><span class="sxs-lookup"><span data-stu-id="cd6b4-107">Method</span></span>                                                                       | <span data-ttu-id="cd6b4-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cd6b4-108">Return Type</span></span>                                                   | <span data-ttu-id="cd6b4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cd6b4-109">Description</span></span>                                                                                  |
| :--------------------------------------------------------------------------- | :------------------------------------------------------------ | :------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="cd6b4-110">Перечисление applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="cd6b4-110">List applicationTemplate</span></span>](../api/applicationtemplate-list.md)               | [<span data-ttu-id="cd6b4-111">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="cd6b4-111">applicationTemplate</span></span>](applicationtemplate.md)                 | <span data-ttu-id="cd6b4-112">Получение списка объектов applicationTemplate.</span><span class="sxs-lookup"><span data-stu-id="cd6b4-112">Retrieve a list of applicationTemplate objects.</span></span>                                              |
| [<span data-ttu-id="cd6b4-113">Получение applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="cd6b4-113">Get applicationTemplate</span></span>](../api/applicationtemplate-get.md)                 | [<span data-ttu-id="cd6b4-114">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="cd6b4-114">applicationTemplate</span></span>](applicationtemplate.md)                 | <span data-ttu-id="cd6b4-115">Чтение свойств и связей объекта applicationTemplate.</span><span class="sxs-lookup"><span data-stu-id="cd6b4-115">Read properties and relationships of applicationTemplate object.</span></span>                             |
| [<span data-ttu-id="cd6b4-116">Создание экземпляра applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="cd6b4-116">Instantiate applicationTemplate</span></span>](../api/applicationtemplate-instantiate.md) | [<span data-ttu-id="cd6b4-117">applicationServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="cd6b4-117">applicationServicePrincipal</span></span>](applicationserviceprincipal.md) | <span data-ttu-id="cd6b4-118">Добавьте экземпляр приложения из галереи приложений Azure AD в каталог.</span><span class="sxs-lookup"><span data-stu-id="cd6b4-118">Add an instance of an application from the Azure AD application gallery into your directory.</span></span> |

## <a name="properties"></a><span data-ttu-id="cd6b4-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd6b4-119">Properties</span></span>

| <span data-ttu-id="cd6b4-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd6b4-120">Property</span></span>                   | <span data-ttu-id="cd6b4-121">Тип</span><span class="sxs-lookup"><span data-stu-id="cd6b4-121">Type</span></span>              | <span data-ttu-id="cd6b4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cd6b4-122">Description</span></span>                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| :------------------------- | :---------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="cd6b4-123">categories</span><span class="sxs-lookup"><span data-stu-id="cd6b4-123">categories</span></span>                 | <span data-ttu-id="cd6b4-124">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cd6b4-124">String collection</span></span> | <span data-ttu-id="cd6b4-125">Список категорий для приложения.</span><span class="sxs-lookup"><span data-stu-id="cd6b4-125">The list of categories for the application.</span></span> <span data-ttu-id="cd6b4-126">Поддерживаемые значения могут быть: `Collaboration` `Business Management` , `Consumer` `Content management` `CRM` `Data services` `Developer services` `E-commerce` `Education` , `ERP` `Finance` и `Health` `Human resources` `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Project management` `Telecommunications` `Tools, Travel` `Web design & hosting` .</span><span class="sxs-lookup"><span data-stu-id="cd6b4-126">Supported values can be: `Collaboration`, `Business Management`, `Consumer`,`Content management`, `CRM`, `Data services`, `Developer services`, `E-commerce`, `Education`, `ERP`, `Finance`, `Health`, `Human resources`, `IT infrastructure`, `Mail`, `Management`, `Marketing`, `Media`, `Productivity`, `Project management`, `Telecommunications`, `Tools, Travel`, and `Web design & hosting`.</span></span> |
| <span data-ttu-id="cd6b4-127">description</span><span class="sxs-lookup"><span data-stu-id="cd6b4-127">description</span></span>                | <span data-ttu-id="cd6b4-128">String</span><span class="sxs-lookup"><span data-stu-id="cd6b4-128">String</span></span>            | <span data-ttu-id="cd6b4-129">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="cd6b4-129">A description of the application.</span></span>                                                                                                                                                                                                                                                                                                                                                                                                               |
| <span data-ttu-id="cd6b4-130">displayName</span><span class="sxs-lookup"><span data-stu-id="cd6b4-130">displayName</span></span>                | <span data-ttu-id="cd6b4-131">String</span><span class="sxs-lookup"><span data-stu-id="cd6b4-131">String</span></span>            | <span data-ttu-id="cd6b4-132">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="cd6b4-132">The name of the application.</span></span>                                                                                                                                                                                                                                                                                                                                                                                                                    |
| <span data-ttu-id="cd6b4-133">homePageUrl</span><span class="sxs-lookup"><span data-stu-id="cd6b4-133">homePageUrl</span></span>                | <span data-ttu-id="cd6b4-134">String</span><span class="sxs-lookup"><span data-stu-id="cd6b4-134">String</span></span>            | <span data-ttu-id="cd6b4-135">URL-адрес домашней страницы приложения.</span><span class="sxs-lookup"><span data-stu-id="cd6b4-135">The home page URL of the application.</span></span>                                                                                                                                                                                                                                                                                                                                                                                                           |
| <span data-ttu-id="cd6b4-136">id</span><span class="sxs-lookup"><span data-stu-id="cd6b4-136">id</span></span>                         | <span data-ttu-id="cd6b4-137">String</span><span class="sxs-lookup"><span data-stu-id="cd6b4-137">String</span></span>            | <span data-ttu-id="cd6b4-138">Уникальный идентификатор для приложения.</span><span class="sxs-lookup"><span data-stu-id="cd6b4-138">Unique identifier for the application.</span></span> <span data-ttu-id="cd6b4-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd6b4-139">Read-only.</span></span>                                                                                                                                                                                                                                                                                                                                                                                               |
| <span data-ttu-id="cd6b4-140">logoUrl</span><span class="sxs-lookup"><span data-stu-id="cd6b4-140">logoUrl</span></span>                    | <span data-ttu-id="cd6b4-141">String</span><span class="sxs-lookup"><span data-stu-id="cd6b4-141">String</span></span>            | <span data-ttu-id="cd6b4-142">URL-адрес для получения логотипа для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="cd6b4-142">The URL to get the logo for this application.</span></span>                                                                                                                                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="cd6b4-143">publisher</span><span class="sxs-lookup"><span data-stu-id="cd6b4-143">publisher</span></span>                  | <span data-ttu-id="cd6b4-144">String</span><span class="sxs-lookup"><span data-stu-id="cd6b4-144">String</span></span>            | <span data-ttu-id="cd6b4-145">Имя издателя для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="cd6b4-145">The name of the publisher for this application.</span></span>                                                                                                                                                                                                                                                                                                                                                                                                 |
| <span data-ttu-id="cd6b4-146">supportedProvisioningTypes</span><span class="sxs-lookup"><span data-stu-id="cd6b4-146">supportedProvisioningTypes</span></span> | <span data-ttu-id="cd6b4-147">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cd6b4-147">String collection</span></span> | <span data-ttu-id="cd6b4-148">Список режимов подготовка, поддерживаемых этим приложением.</span><span class="sxs-lookup"><span data-stu-id="cd6b4-148">The list of provisioning modes supported by this application.</span></span> <span data-ttu-id="cd6b4-149">Единственным допустимым значением `sync` является .</span><span class="sxs-lookup"><span data-stu-id="cd6b4-149">The only valid value is `sync`.</span></span>                                                                                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="cd6b4-150">supportedSingleSignOnModes</span><span class="sxs-lookup"><span data-stu-id="cd6b4-150">supportedSingleSignOnModes</span></span> | <span data-ttu-id="cd6b4-151">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cd6b4-151">String collection</span></span> | <span data-ttu-id="cd6b4-152">Список режимов единой регистрации, поддерживаемых этим приложением.</span><span class="sxs-lookup"><span data-stu-id="cd6b4-152">The list of single sign-on modes supported by this application.</span></span> <span data-ttu-id="cd6b4-153">Поддерживаемые значения: `oidc`, `password`, `saml` и `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="cd6b4-153">The supported values are `oidc`, `password`, `saml`, and `notSupported`.</span></span>                                                                                                                                                                                                                                                                                                            |

## <a name="relationships"></a><span data-ttu-id="cd6b4-154">Связи</span><span class="sxs-lookup"><span data-stu-id="cd6b4-154">Relationships</span></span>

<span data-ttu-id="cd6b4-155">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cd6b4-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd6b4-156">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cd6b4-156">JSON representation</span></span>

<span data-ttu-id="cd6b4-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd6b4-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationTemplate",
  "keyProperty": "id"
}-->

```json
{
  "id": "id-value",
  "displayName": "displayName-value",
  "homePageUrl": "homePageUrl-value",
  "supportedSingleSignOnModes": ["supportedSingleSignOnModes-value"],
  "logoUrl": "logoUrl-value",
  "categories": ["categories-value"],
  "publisher": "publisher-value",
  "description": "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
