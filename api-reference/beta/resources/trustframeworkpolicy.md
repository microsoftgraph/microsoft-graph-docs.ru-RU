---
title: трустфрамеворкполици
description: В политике Azure AD B2C Trust Framework называются пользовательскими политиками. В этом разделе описываются операции, доступные в объекте Трустфрамеворкполици для клиента.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 553463811f74a536cd3be5317718e00f91c95260
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218046"
---
# <a name="trustframeworkpolicy-resource-type"></a><span data-ttu-id="972a6-104">Тип ресурса Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="972a6-104">trustFrameworkPolicy resource type</span></span>

<span data-ttu-id="972a6-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="972a6-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="972a6-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="972a6-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="972a6-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="972a6-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="972a6-108">Представляет политику [платформы доверия](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) (также называемую [настраиваемой политикой](/azure/active-directory-b2c/active-directory-b2c-overview-custom)) в [Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview).</span><span class="sxs-lookup"><span data-stu-id="972a6-108">Represents a [Trust Framework](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) policy (also called [custom policy](/azure/active-directory-b2c/active-directory-b2c-overview-custom)) in [Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview).</span></span> <span data-ttu-id="972a6-109">Политика инфраструктуры доверия предоставляет полный контроль над путешествием пользователей.</span><span class="sxs-lookup"><span data-stu-id="972a6-109">A Trust Framework policy gives full control over the user journeys.</span></span> <span data-ttu-id="972a6-110">Используйте его для:</span><span class="sxs-lookup"><span data-stu-id="972a6-110">Use it to:</span></span>

* <span data-ttu-id="972a6-111">Полностью настройте вход и вход в систему.</span><span class="sxs-lookup"><span data-stu-id="972a6-111">Customize the sign-up and sign-in experiences fully.</span></span>
* <span data-ttu-id="972a6-112">Федерацию на любой поставщик удостоверений SAML, Open ID Connect или OAuth2.</span><span class="sxs-lookup"><span data-stu-id="972a6-112">Federate to any SAML, Open ID Connect, or OAuth2 identity provider.</span></span>
* <span data-ttu-id="972a6-113">Интеграция с другими системами или хранилищами пользовательских данных путем вызова конечных точек REST.</span><span class="sxs-lookup"><span data-stu-id="972a6-113">Integrate with other systems or user data stores by calling REST endpoints.</span></span>
* <span data-ttu-id="972a6-114">Преобразование утверждений и настройка маркеров, выданных приложению проверяющей стороны.</span><span class="sxs-lookup"><span data-stu-id="972a6-114">Transform claims and customize tokens issued to the relying party application.</span></span>

<span data-ttu-id="972a6-115">Для получения дополнительных сведений см. [настраиваемые политики в Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span><span class="sxs-lookup"><span data-stu-id="972a6-115">For more information, see [Custom policies in Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span></span>

## <a name="methods"></a><span data-ttu-id="972a6-116">Методы</span><span class="sxs-lookup"><span data-stu-id="972a6-116">Methods</span></span>

| <span data-ttu-id="972a6-117">Метод</span><span class="sxs-lookup"><span data-stu-id="972a6-117">Method</span></span>       | <span data-ttu-id="972a6-118">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="972a6-118">Return Type</span></span>  |<span data-ttu-id="972a6-119">Описание</span><span class="sxs-lookup"><span data-stu-id="972a6-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="972a6-120">Создание Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="972a6-120">Create trustFrameworkPolicy</span></span>](../api/trustframework-post-trustframeworkpolicy.md)|<span data-ttu-id="972a6-121">трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="972a6-121">trustFrameworkPolicy</span></span>|<span data-ttu-id="972a6-122">Создание нового Трустфрамеворкполици.</span><span class="sxs-lookup"><span data-stu-id="972a6-122">Create a new trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="972a6-123">Получение Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="972a6-123">Get trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-get.md) |<span data-ttu-id="972a6-124">трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="972a6-124">trustFrameworkPolicy</span></span>|<span data-ttu-id="972a6-125">Чтение свойств существующего Трустфрамеворкполици.</span><span class="sxs-lookup"><span data-stu-id="972a6-125">Read properties of an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="972a6-126">Список ТрустфрамеворкполиЦиес</span><span class="sxs-lookup"><span data-stu-id="972a6-126">List trustFrameworkPolicies</span></span>](../api/trustframework-list-trustframeworkpolicies.md)|<span data-ttu-id="972a6-127">Коллекция Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="972a6-127">trustFrameworkPolicy collection</span></span>|<span data-ttu-id="972a6-128">Список всех ТрустфрамеворкполиЦиес, настроенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="972a6-128">List all trustFrameworkPolicies configured in a tenant.</span></span>|
|[<span data-ttu-id="972a6-129">Обновление или создание Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="972a6-129">Update or create trustFrameworkPolicy</span></span>](../api/trustframework-put-trustframeworkpolicy.md)|<span data-ttu-id="972a6-130">Нет</span><span class="sxs-lookup"><span data-stu-id="972a6-130">None</span></span>|<span data-ttu-id="972a6-131">Обновление существующего Трустфрамеворкполици.</span><span class="sxs-lookup"><span data-stu-id="972a6-131">Update an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="972a6-132">Удаление Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="972a6-132">Delete trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-delete.md)|<span data-ttu-id="972a6-133">Нет</span><span class="sxs-lookup"><span data-stu-id="972a6-133">None</span></span>|<span data-ttu-id="972a6-134">Удаление существующего Трустфрамеворкполици.</span><span class="sxs-lookup"><span data-stu-id="972a6-134">Delete an existing trustFrameworkPolicy.</span></span>|

## <a name="properties"></a><span data-ttu-id="972a6-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="972a6-135">Properties</span></span>

|<span data-ttu-id="972a6-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="972a6-136">Property</span></span>|<span data-ttu-id="972a6-137">Тип</span><span class="sxs-lookup"><span data-stu-id="972a6-137">Type</span></span>|<span data-ttu-id="972a6-138">Описание</span><span class="sxs-lookup"><span data-stu-id="972a6-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="972a6-139">id</span><span class="sxs-lookup"><span data-stu-id="972a6-139">id</span></span>|<span data-ttu-id="972a6-140">String</span><span class="sxs-lookup"><span data-stu-id="972a6-140">String</span></span>|<span data-ttu-id="972a6-141">Идентификатор политики.</span><span class="sxs-lookup"><span data-stu-id="972a6-141">The ID of the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="972a6-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="972a6-142">JSON representation</span></span>

<span data-ttu-id="972a6-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="972a6-143">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType":"microsoft.graph.entity",
  "keyProperty":"id",
  "isMediaEntity":true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
}-->
```json
{
   "id": "B2C_1A_Test"
}
```

## <a name="see-also"></a><span data-ttu-id="972a6-144">См. также</span><span class="sxs-lookup"><span data-stu-id="972a6-144">See also</span></span>

- <span data-ttu-id="972a6-145">[схема трустфрамеворкполици](/azure/active-directory-b2c/trustframeworkpolicy) для получения сведений об элементах схемы.</span><span class="sxs-lookup"><span data-stu-id="972a6-145">[trustFrameworkPolicy schema](/azure/active-directory-b2c/trustframeworkpolicy) for information about the schema elements.</span></span>
- [<span data-ttu-id="972a6-146">Трустфрамеворкполици. xsd</span><span class="sxs-lookup"><span data-stu-id="972a6-146">trustFrameworkPolicy.xsd</span></span>](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)
