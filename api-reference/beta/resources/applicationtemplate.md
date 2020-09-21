---
title: Тип ресурса Аппликатионтемплате
description: Представляет приложение в коллекции приложений Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1dcb5d1a4f1a86521081487ec66494d76c035b82
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050236"
---
# <a name="applicationtemplate-resource-type"></a><span data-ttu-id="a0a0a-103">Тип ресурса Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="a0a0a-103">applicationTemplate resource type</span></span>

<span data-ttu-id="a0a0a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0a0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0a0a-105">Представляет приложение в [коллекции приложений Azure AD](/azure/active-directory/saas-apps/tutorial-list).</span><span class="sxs-lookup"><span data-stu-id="a0a0a-105">Represents an application in the [Azure AD application gallery](/azure/active-directory/saas-apps/tutorial-list).</span></span>

## <a name="methods"></a><span data-ttu-id="a0a0a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a0a0a-106">Methods</span></span>

| <span data-ttu-id="a0a0a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a0a0a-107">Method</span></span>       | <span data-ttu-id="a0a0a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a0a0a-108">Return Type</span></span> | <span data-ttu-id="a0a0a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a0a0a-109">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="a0a0a-110">Перечисление applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="a0a0a-110">List applicationTemplate</span></span>](../api/applicationtemplate-list.md)|[<span data-ttu-id="a0a0a-111">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="a0a0a-111">applicationTemplate</span></span>](applicationtemplate.md)|<span data-ttu-id="a0a0a-112">Получение списка объектов Аппликатионтемплате.</span><span class="sxs-lookup"><span data-stu-id="a0a0a-112">Retrieve a list of applicationTemplate objects.</span></span>|
| [<span data-ttu-id="a0a0a-113">Получение Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="a0a0a-113">Get applicationTemplate</span></span>](../api/applicationtemplate-get.md) | [<span data-ttu-id="a0a0a-114">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="a0a0a-114">applicationTemplate</span></span>](applicationtemplate.md) | <span data-ttu-id="a0a0a-115">Чтение свойств и связей объекта Аппликатионтемплате.</span><span class="sxs-lookup"><span data-stu-id="a0a0a-115">Read properties and relationships of applicationTemplate object.</span></span> |
|[<span data-ttu-id="a0a0a-116">Создание экземпляра applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="a0a0a-116">Instantiate applicationTemplate</span></span>](../api/applicationtemplate-instantiate.md)|[<span data-ttu-id="a0a0a-117">аппликатионсервицепринЦипал</span><span class="sxs-lookup"><span data-stu-id="a0a0a-117">applicationServicePrincipal</span></span>](applicationserviceprincipal.md)| <span data-ttu-id="a0a0a-118">Добавьте экземпляр приложения из коллекции приложений Azure AD в ваш каталог.</span><span class="sxs-lookup"><span data-stu-id="a0a0a-118">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>|


## <a name="properties"></a><span data-ttu-id="a0a0a-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0a0a-119">Properties</span></span>

| <span data-ttu-id="a0a0a-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0a0a-120">Property</span></span>     | <span data-ttu-id="a0a0a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a0a0a-121">Type</span></span>        | <span data-ttu-id="a0a0a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a0a0a-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a0a0a-123">categories</span><span class="sxs-lookup"><span data-stu-id="a0a0a-123">categories</span></span>|<span data-ttu-id="a0a0a-124">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a0a0a-124">String collection</span></span>|<span data-ttu-id="a0a0a-125">Список категорий для приложения.</span><span class="sxs-lookup"><span data-stu-id="a0a0a-125">The list of categories for the application.</span></span> <span data-ttu-id="a0a0a-126">Поддерживаются следующие значения:,,,,,,,,,, `Collaboration` `Business Management` `Consumer` `Content management` `CRM` `Data services` `Developer services` `E-commerce` `Education` `ERP` `Finance` `Health` , `Human resources` , `IT infrastructure` , `Mail` `Management` `Marketing` `Media` `Productivity` `Project management` `Telecommunications` `Tools, Travel` `Web design & hosting` ,,,,,,,,,,,,,, и.</span><span class="sxs-lookup"><span data-stu-id="a0a0a-126">Supported values can be: `Collaboration`, `Business Management`, `Consumer`,`Content management`, `CRM`, `Data services`, `Developer services`, `E-commerce`, `Education`, `ERP`, `Finance`, `Health`, `Human resources`, `IT infrastructure`, `Mail`, `Management`, `Marketing`, `Media`, `Productivity`, `Project management`, `Telecommunications`, `Tools, Travel`, and `Web design & hosting`.</span></span>|
|<span data-ttu-id="a0a0a-127">description</span><span class="sxs-lookup"><span data-stu-id="a0a0a-127">description</span></span>|<span data-ttu-id="a0a0a-128">String</span><span class="sxs-lookup"><span data-stu-id="a0a0a-128">String</span></span>|<span data-ttu-id="a0a0a-129">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a0a0a-129">A description of the application.</span></span>|
|<span data-ttu-id="a0a0a-130">displayName</span><span class="sxs-lookup"><span data-stu-id="a0a0a-130">displayName</span></span>|<span data-ttu-id="a0a0a-131">Строка</span><span class="sxs-lookup"><span data-stu-id="a0a0a-131">String</span></span>|<span data-ttu-id="a0a0a-132">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="a0a0a-132">The name of the application.</span></span>|
|<span data-ttu-id="a0a0a-133">хомепажеурл</span><span class="sxs-lookup"><span data-stu-id="a0a0a-133">homePageUrl</span></span>|<span data-ttu-id="a0a0a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a0a0a-134">String</span></span>|<span data-ttu-id="a0a0a-135">URL-адрес домашней страницы приложения.</span><span class="sxs-lookup"><span data-stu-id="a0a0a-135">The home page URL of the application.</span></span>|
|<span data-ttu-id="a0a0a-136">id</span><span class="sxs-lookup"><span data-stu-id="a0a0a-136">id</span></span>|<span data-ttu-id="a0a0a-137">Строка</span><span class="sxs-lookup"><span data-stu-id="a0a0a-137">String</span></span>| <span data-ttu-id="a0a0a-138">Уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="a0a0a-138">Unique identifier for the application.</span></span> <span data-ttu-id="a0a0a-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a0a0a-139">Read-only.</span></span>|
|<span data-ttu-id="a0a0a-140">logoUrl</span><span class="sxs-lookup"><span data-stu-id="a0a0a-140">logoUrl</span></span>|<span data-ttu-id="a0a0a-141">Строка</span><span class="sxs-lookup"><span data-stu-id="a0a0a-141">String</span></span>|<span data-ttu-id="a0a0a-142">URL-адрес для получения логотипа для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="a0a0a-142">The URL to get the logo for this application.</span></span>|
|<span data-ttu-id="a0a0a-143">publisher</span><span class="sxs-lookup"><span data-stu-id="a0a0a-143">publisher</span></span>|<span data-ttu-id="a0a0a-144">String</span><span class="sxs-lookup"><span data-stu-id="a0a0a-144">String</span></span>|<span data-ttu-id="a0a0a-145">Имя издателя для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="a0a0a-145">The name of the publisher for this application.</span></span>|
|<span data-ttu-id="a0a0a-146">суппортедпровисионингтипес</span><span class="sxs-lookup"><span data-stu-id="a0a0a-146">supportedProvisioningTypes</span></span>|<span data-ttu-id="a0a0a-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a0a0a-147">String collection</span></span>|<span data-ttu-id="a0a0a-148">Список режимов подготовки, поддерживаемых этим приложением.</span><span class="sxs-lookup"><span data-stu-id="a0a0a-148">The list of provisioning modes supported by this application.</span></span> <span data-ttu-id="a0a0a-149">Единственное допустимое значение: `sync` .</span><span class="sxs-lookup"><span data-stu-id="a0a0a-149">The only valid value is `sync`.</span></span>|
|<span data-ttu-id="a0a0a-150">суппортедсинглесигнонмодес</span><span class="sxs-lookup"><span data-stu-id="a0a0a-150">supportedSingleSignOnModes</span></span>|<span data-ttu-id="a0a0a-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a0a0a-151">String collection</span></span>|<span data-ttu-id="a0a0a-152">Список режимов единого входа, поддерживаемых этим приложением.</span><span class="sxs-lookup"><span data-stu-id="a0a0a-152">The list of single sign-on modes supported by this application.</span></span> <span data-ttu-id="a0a0a-153">Поддерживаемые значения: `password` ,, `saml` `external` и `oidc` .</span><span class="sxs-lookup"><span data-stu-id="a0a0a-153">The supported values are `password`, `saml`, `external`, and `oidc`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0a0a-154">Связи</span><span class="sxs-lookup"><span data-stu-id="a0a0a-154">Relationships</span></span>

<span data-ttu-id="a0a0a-155">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a0a0a-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0a0a-156">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a0a0a-156">JSON representation</span></span>

<span data-ttu-id="a0a0a-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0a0a-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationTemplate",
  "baseType": "",
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


