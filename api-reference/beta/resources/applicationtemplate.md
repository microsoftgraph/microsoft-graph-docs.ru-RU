---
title: Тип ресурса applicationTemplate
description: Представляет приложение в коллекции приложений Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 37468877721b9ac534c0118aeb93fd613fca7f88
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159180"
---
# <a name="applicationtemplate-resource-type"></a><span data-ttu-id="dc67b-103">Тип ресурса applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="dc67b-103">applicationTemplate resource type</span></span>

<span data-ttu-id="dc67b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc67b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc67b-105">Представляет приложение в коллекции [приложений Azure AD.](/azure/active-directory/saas-apps/tutorial-list)</span><span class="sxs-lookup"><span data-stu-id="dc67b-105">Represents an application in the [Azure AD application gallery](/azure/active-directory/saas-apps/tutorial-list).</span></span>

## <a name="methods"></a><span data-ttu-id="dc67b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="dc67b-106">Methods</span></span>

| <span data-ttu-id="dc67b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="dc67b-107">Method</span></span>       | <span data-ttu-id="dc67b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dc67b-108">Return Type</span></span> | <span data-ttu-id="dc67b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dc67b-109">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="dc67b-110">Перечисление applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="dc67b-110">List applicationTemplate</span></span>](../api/applicationtemplate-list.md)|[<span data-ttu-id="dc67b-111">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="dc67b-111">applicationTemplate</span></span>](applicationtemplate.md)|<span data-ttu-id="dc67b-112">Получение списка объектов applicationTemplate.</span><span class="sxs-lookup"><span data-stu-id="dc67b-112">Retrieve a list of applicationTemplate objects.</span></span>|
| [<span data-ttu-id="dc67b-113">Получение applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="dc67b-113">Get applicationTemplate</span></span>](../api/applicationtemplate-get.md) | [<span data-ttu-id="dc67b-114">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="dc67b-114">applicationTemplate</span></span>](applicationtemplate.md) | <span data-ttu-id="dc67b-115">Чтение свойств и связей объекта applicationTemplate.</span><span class="sxs-lookup"><span data-stu-id="dc67b-115">Read properties and relationships of applicationTemplate object.</span></span> |
|[<span data-ttu-id="dc67b-116">Создание экземпляра applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="dc67b-116">Instantiate applicationTemplate</span></span>](../api/applicationtemplate-instantiate.md)|[<span data-ttu-id="dc67b-117">applicationServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="dc67b-117">applicationServicePrincipal</span></span>](applicationserviceprincipal.md)| <span data-ttu-id="dc67b-118">Добавьте экземпляр приложения из коллекции приложений Azure AD в каталог.</span><span class="sxs-lookup"><span data-stu-id="dc67b-118">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>|


## <a name="properties"></a><span data-ttu-id="dc67b-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc67b-119">Properties</span></span>

| <span data-ttu-id="dc67b-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc67b-120">Property</span></span>     | <span data-ttu-id="dc67b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="dc67b-121">Type</span></span>        | <span data-ttu-id="dc67b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dc67b-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dc67b-123">categories</span><span class="sxs-lookup"><span data-stu-id="dc67b-123">categories</span></span>|<span data-ttu-id="dc67b-124">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dc67b-124">String collection</span></span>|<span data-ttu-id="dc67b-125">Список категорий для приложения.</span><span class="sxs-lookup"><span data-stu-id="dc67b-125">The list of categories for the application.</span></span> <span data-ttu-id="dc67b-126">Поддерживаемые значения: `Collaboration` , , , , `Business Management` `Consumer` , `Content management` , , `CRM` , , `Data services` , `Developer services` `E-commerce` `Education` `ERP` `Finance` `Health` `Human resources` и `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Project management` `Telecommunications` `Tools, Travel` `Web design & hosting` .</span><span class="sxs-lookup"><span data-stu-id="dc67b-126">Supported values can be: `Collaboration`, `Business Management`, `Consumer`,`Content management`, `CRM`, `Data services`, `Developer services`, `E-commerce`, `Education`, `ERP`, `Finance`, `Health`, `Human resources`, `IT infrastructure`, `Mail`, `Management`, `Marketing`, `Media`, `Productivity`, `Project management`, `Telecommunications`, `Tools, Travel`, and `Web design & hosting`.</span></span>|
|<span data-ttu-id="dc67b-127">description</span><span class="sxs-lookup"><span data-stu-id="dc67b-127">description</span></span>|<span data-ttu-id="dc67b-128">String</span><span class="sxs-lookup"><span data-stu-id="dc67b-128">String</span></span>|<span data-ttu-id="dc67b-129">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="dc67b-129">A description of the application.</span></span>|
|<span data-ttu-id="dc67b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="dc67b-130">displayName</span></span>|<span data-ttu-id="dc67b-131">String</span><span class="sxs-lookup"><span data-stu-id="dc67b-131">String</span></span>|<span data-ttu-id="dc67b-132">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="dc67b-132">The name of the application.</span></span>|
|<span data-ttu-id="dc67b-133">homePageUrl</span><span class="sxs-lookup"><span data-stu-id="dc67b-133">homePageUrl</span></span>|<span data-ttu-id="dc67b-134">String</span><span class="sxs-lookup"><span data-stu-id="dc67b-134">String</span></span>|<span data-ttu-id="dc67b-135">URL-адрес домашней страницы приложения.</span><span class="sxs-lookup"><span data-stu-id="dc67b-135">The home page URL of the application.</span></span>|
|<span data-ttu-id="dc67b-136">id</span><span class="sxs-lookup"><span data-stu-id="dc67b-136">id</span></span>|<span data-ttu-id="dc67b-137">String</span><span class="sxs-lookup"><span data-stu-id="dc67b-137">String</span></span>| <span data-ttu-id="dc67b-138">Уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="dc67b-138">Unique identifier for the application.</span></span> <span data-ttu-id="dc67b-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc67b-139">Read-only.</span></span>|
|<span data-ttu-id="dc67b-140">logoUrl</span><span class="sxs-lookup"><span data-stu-id="dc67b-140">logoUrl</span></span>|<span data-ttu-id="dc67b-141">String</span><span class="sxs-lookup"><span data-stu-id="dc67b-141">String</span></span>|<span data-ttu-id="dc67b-142">URL-адрес для получения логотипа для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="dc67b-142">The URL to get the logo for this application.</span></span>|
|<span data-ttu-id="dc67b-143">publisher</span><span class="sxs-lookup"><span data-stu-id="dc67b-143">publisher</span></span>|<span data-ttu-id="dc67b-144">String</span><span class="sxs-lookup"><span data-stu-id="dc67b-144">String</span></span>|<span data-ttu-id="dc67b-145">Имя издателя для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="dc67b-145">The name of the publisher for this application.</span></span>|
|<span data-ttu-id="dc67b-146">supportedProvisioningTypes</span><span class="sxs-lookup"><span data-stu-id="dc67b-146">supportedProvisioningTypes</span></span>|<span data-ttu-id="dc67b-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dc67b-147">String collection</span></span>|<span data-ttu-id="dc67b-148">Список режимов предоставления, поддерживаемых этим приложением.</span><span class="sxs-lookup"><span data-stu-id="dc67b-148">The list of provisioning modes supported by this application.</span></span> <span data-ttu-id="dc67b-149">Единственным допустимым значением `sync` является .</span><span class="sxs-lookup"><span data-stu-id="dc67b-149">The only valid value is `sync`.</span></span>|
|<span data-ttu-id="dc67b-150">supportedSingleSignOnModes</span><span class="sxs-lookup"><span data-stu-id="dc67b-150">supportedSingleSignOnModes</span></span>|<span data-ttu-id="dc67b-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dc67b-151">String collection</span></span>|<span data-ttu-id="dc67b-152">Список режимов единого входов, поддерживаемых этим приложением.</span><span class="sxs-lookup"><span data-stu-id="dc67b-152">The list of single sign-on modes supported by this application.</span></span> <span data-ttu-id="dc67b-153">Поддерживаемые значения: `password`, `saml`, `external` и `oidc`.</span><span class="sxs-lookup"><span data-stu-id="dc67b-153">The supported values are `password`, `saml`, `external`, and `oidc`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc67b-154">Связи</span><span class="sxs-lookup"><span data-stu-id="dc67b-154">Relationships</span></span>

<span data-ttu-id="dc67b-155">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="dc67b-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc67b-156">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dc67b-156">JSON representation</span></span>

<span data-ttu-id="dc67b-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc67b-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationTemplate",
  "keyProperty": "id"
}-->

```json
{
    "id" : "id-value",
    "displayName" : "displayName-value",
    "homePageUrl" : "homePageUrl-value",
    "supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
    "logoUrl" : "logoUrl-value",
    "categories" : ["categories-value"],
    "publisher" : "publisher-value",
    "description" : "description-value"
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



