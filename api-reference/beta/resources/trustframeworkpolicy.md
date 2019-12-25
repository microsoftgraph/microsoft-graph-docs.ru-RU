---
title: трустфрамеворкполици
description: В политике Azure AD B2C Trust Framework называются пользовательскими политиками. В этом разделе описываются операции, доступные в объекте Трустфрамеворкполици для клиента.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 83b4a747007ed0ba55cc0fec37b9cf45debf1f47
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866506"
---
# <a name="trustframeworkpolicy-resource-type"></a><span data-ttu-id="0d98c-104">Тип ресурса Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="0d98c-104">trustFrameworkPolicy resource type</span></span>

> <span data-ttu-id="0d98c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0d98c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d98c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d98c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0d98c-107">Представляет политику [платформы доверия](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) (также называемую [настраиваемой политикой](/azure/active-directory-b2c/active-directory-b2c-overview-custom)) в [Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview).</span><span class="sxs-lookup"><span data-stu-id="0d98c-107">Represents a [Trust Framework](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) policy (also called [custom policy](/azure/active-directory-b2c/active-directory-b2c-overview-custom)) in [Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview).</span></span> <span data-ttu-id="0d98c-108">Политика инфраструктуры доверия предоставляет полный контроль над путешествием пользователей.</span><span class="sxs-lookup"><span data-stu-id="0d98c-108">A Trust Framework policy gives full control over the user journeys.</span></span> <span data-ttu-id="0d98c-109">Используйте его для:</span><span class="sxs-lookup"><span data-stu-id="0d98c-109">Use it to:</span></span>

* <span data-ttu-id="0d98c-110">Полностью настройте вход и вход в систему.</span><span class="sxs-lookup"><span data-stu-id="0d98c-110">Customize the sign-up and sign-in experiences fully.</span></span>
* <span data-ttu-id="0d98c-111">Федерацию на любой поставщик удостоверений SAML, Open ID Connect или OAuth2.</span><span class="sxs-lookup"><span data-stu-id="0d98c-111">Federate to any SAML, Open ID Connect, or OAuth2 identity provider.</span></span>
* <span data-ttu-id="0d98c-112">Интеграция с другими системами или хранилищами пользовательских данных путем вызова конечных точек REST.</span><span class="sxs-lookup"><span data-stu-id="0d98c-112">Integrate with other systems or user data stores by calling REST endpoints.</span></span>
* <span data-ttu-id="0d98c-113">Преобразование утверждений и настройка маркеров, выданных приложению проверяющей стороны.</span><span class="sxs-lookup"><span data-stu-id="0d98c-113">Transform claims and customize tokens issued to the relying party application.</span></span>

<span data-ttu-id="0d98c-114">Для получения дополнительных сведений см. [настраиваемые политики в Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span><span class="sxs-lookup"><span data-stu-id="0d98c-114">For more information, see [Custom policies in Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span></span>

## <a name="methods"></a><span data-ttu-id="0d98c-115">Методы</span><span class="sxs-lookup"><span data-stu-id="0d98c-115">Methods</span></span>

| <span data-ttu-id="0d98c-116">Метод</span><span class="sxs-lookup"><span data-stu-id="0d98c-116">Method</span></span>       | <span data-ttu-id="0d98c-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0d98c-117">Return Type</span></span>  |<span data-ttu-id="0d98c-118">Описание</span><span class="sxs-lookup"><span data-stu-id="0d98c-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0d98c-119">Создание Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="0d98c-119">Create trustFrameworkPolicy</span></span>](../api/trustframework-post-trustframeworkpolicy.md)|<span data-ttu-id="0d98c-120">трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="0d98c-120">trustFrameworkPolicy</span></span>|<span data-ttu-id="0d98c-121">Создание нового Трустфрамеворкполици.</span><span class="sxs-lookup"><span data-stu-id="0d98c-121">Create a new trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="0d98c-122">Получение Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="0d98c-122">Get trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-get.md) |<span data-ttu-id="0d98c-123">трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="0d98c-123">trustFrameworkPolicy</span></span>|<span data-ttu-id="0d98c-124">Чтение свойств существующего Трустфрамеворкполици.</span><span class="sxs-lookup"><span data-stu-id="0d98c-124">Read properties of an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="0d98c-125">Список ТрустфрамеворкполиЦиес</span><span class="sxs-lookup"><span data-stu-id="0d98c-125">List trustFrameworkPolicies</span></span>](../api/trustframework-list-trustframeworkpolicies.md)|<span data-ttu-id="0d98c-126">Коллекция Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="0d98c-126">trustFrameworkPolicy collection</span></span>|<span data-ttu-id="0d98c-127">Список всех ТрустфрамеворкполиЦиес, настроенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="0d98c-127">List all trustFrameworkPolicies configured in a tenant.</span></span>|
|[<span data-ttu-id="0d98c-128">Обновление или создание Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="0d98c-128">Update or create trustFrameworkPolicy</span></span>](../api/trustframework-put-trustframeworkpolicy.md)|<span data-ttu-id="0d98c-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="0d98c-129">None</span></span>|<span data-ttu-id="0d98c-130">Обновление существующего Трустфрамеворкполици.</span><span class="sxs-lookup"><span data-stu-id="0d98c-130">Update an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="0d98c-131">Удаление Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="0d98c-131">Delete trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-delete.md)|<span data-ttu-id="0d98c-132">Нет.</span><span class="sxs-lookup"><span data-stu-id="0d98c-132">None</span></span>|<span data-ttu-id="0d98c-133">Удаление существующего Трустфрамеворкполици.</span><span class="sxs-lookup"><span data-stu-id="0d98c-133">Delete an existing trustFrameworkPolicy.</span></span>|

## <a name="properties"></a><span data-ttu-id="0d98c-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d98c-134">Properties</span></span>

|<span data-ttu-id="0d98c-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d98c-135">Property</span></span>|<span data-ttu-id="0d98c-136">Тип</span><span class="sxs-lookup"><span data-stu-id="0d98c-136">Type</span></span>|<span data-ttu-id="0d98c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="0d98c-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d98c-138">id</span><span class="sxs-lookup"><span data-stu-id="0d98c-138">id</span></span>|<span data-ttu-id="0d98c-139">String</span><span class="sxs-lookup"><span data-stu-id="0d98c-139">String</span></span>|<span data-ttu-id="0d98c-140">Идентификатор политики.</span><span class="sxs-lookup"><span data-stu-id="0d98c-140">The ID of the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d98c-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d98c-141">JSON representation</span></span>

<span data-ttu-id="0d98c-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d98c-142">The following is a JSON representation of the resource.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="0d98c-143">См. также</span><span class="sxs-lookup"><span data-stu-id="0d98c-143">See also</span></span>

- <span data-ttu-id="0d98c-144">[схема трустфрамеворкполици](/azure/active-directory-b2c/trustframeworkpolicy) для получения сведений об элементах схемы.</span><span class="sxs-lookup"><span data-stu-id="0d98c-144">[trustFrameworkPolicy schema](/azure/active-directory-b2c/trustframeworkpolicy) for information about the schema elements.</span></span>
- [<span data-ttu-id="0d98c-145">Трустфрамеворкполици. xsd</span><span class="sxs-lookup"><span data-stu-id="0d98c-145">trustFrameworkPolicy.xsd</span></span>](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)
