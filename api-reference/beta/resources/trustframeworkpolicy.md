---
title: trustFrameworkPolicy
description: В политике платформы доверия Azure AD B2C называются настраиваемые политики. В этом описаны операции, доступные для объекта trustFrameworkPolicy для клиента.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a8bb9fc598613d48ac6b9bb34aa02d24872e6300
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442742"
---
# <a name="trustframeworkpolicy-resource-type"></a><span data-ttu-id="dd666-104">тип ресурса trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="dd666-104">trustFrameworkPolicy resource type</span></span>

<span data-ttu-id="dd666-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd666-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd666-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dd666-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd666-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd666-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd666-108">Представляет политику [Trust Framework](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) (также называемую [настраиваемой](/azure/active-directory-b2c/active-directory-b2c-overview-custom)политикой) в Azure Active [Directory B2C.](/azure/active-directory-b2c/active-directory-b2c-overview)</span><span class="sxs-lookup"><span data-stu-id="dd666-108">Represents a [Trust Framework](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) policy (also called [custom policy](/azure/active-directory-b2c/active-directory-b2c-overview-custom)) in [Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview).</span></span> <span data-ttu-id="dd666-109">Политика Trust Framework обеспечивает полный контроль над поездками пользователей.</span><span class="sxs-lookup"><span data-stu-id="dd666-109">A Trust Framework policy gives full control over the user journeys.</span></span> <span data-ttu-id="dd666-110">Используйте его для:</span><span class="sxs-lookup"><span data-stu-id="dd666-110">Use it to:</span></span>

* <span data-ttu-id="dd666-111">Полностью настроить опытом регистрации и регистрации.</span><span class="sxs-lookup"><span data-stu-id="dd666-111">Customize the sign-up and sign-in experiences fully.</span></span>
* <span data-ttu-id="dd666-112">Federate к любому поставщику удостоверений SAML, Open ID Connect или поставщику удостоверений OAuth2.</span><span class="sxs-lookup"><span data-stu-id="dd666-112">Federate to any SAML, Open ID Connect, or OAuth2 identity provider.</span></span>
* <span data-ttu-id="dd666-113">Интеграция с другими системами или хранилищами данных пользователей путем вызова конечных точек REST.</span><span class="sxs-lookup"><span data-stu-id="dd666-113">Integrate with other systems or user data stores by calling REST endpoints.</span></span>
* <span data-ttu-id="dd666-114">Преобразование утверждений и настройка маркеров, выдающихся в приложение-участник.</span><span class="sxs-lookup"><span data-stu-id="dd666-114">Transform claims and customize tokens issued to the relying party application.</span></span>

<span data-ttu-id="dd666-115">Дополнительные сведения см. в [пользовательских политиках в Azure Active Directory B2C.](/azure/active-directory-b2c/active-directory-b2c-overview-custom)</span><span class="sxs-lookup"><span data-stu-id="dd666-115">For more information, see [Custom policies in Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span></span>

## <a name="methods"></a><span data-ttu-id="dd666-116">Методы</span><span class="sxs-lookup"><span data-stu-id="dd666-116">Methods</span></span>

| <span data-ttu-id="dd666-117">Метод</span><span class="sxs-lookup"><span data-stu-id="dd666-117">Method</span></span>       | <span data-ttu-id="dd666-118">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dd666-118">Return Type</span></span>  |<span data-ttu-id="dd666-119">Описание</span><span class="sxs-lookup"><span data-stu-id="dd666-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dd666-120">Создание trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="dd666-120">Create trustFrameworkPolicy</span></span>](../api/trustframework-post-trustframeworkpolicy.md)|<span data-ttu-id="dd666-121">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="dd666-121">trustFrameworkPolicy</span></span>|<span data-ttu-id="dd666-122">Создание нового trustFrameworkPolicy.</span><span class="sxs-lookup"><span data-stu-id="dd666-122">Create a new trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="dd666-123">Get trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="dd666-123">Get trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-get.md) |<span data-ttu-id="dd666-124">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="dd666-124">trustFrameworkPolicy</span></span>|<span data-ttu-id="dd666-125">Чтение свойств существующего trustFrameworkPolicy.</span><span class="sxs-lookup"><span data-stu-id="dd666-125">Read properties of an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="dd666-126">Список trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="dd666-126">List trustFrameworkPolicies</span></span>](../api/trustframework-list-trustframeworkpolicies.md)|<span data-ttu-id="dd666-127">коллекция trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="dd666-127">trustFrameworkPolicy collection</span></span>|<span data-ttu-id="dd666-128">Список всех trustFrameworkPolicies, настроенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="dd666-128">List all trustFrameworkPolicies configured in a tenant.</span></span>|
|[<span data-ttu-id="dd666-129">Обновление или создание trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="dd666-129">Update or create trustFrameworkPolicy</span></span>](../api/trustframework-put-trustframeworkpolicy.md)|<span data-ttu-id="dd666-130">Нет</span><span class="sxs-lookup"><span data-stu-id="dd666-130">None</span></span>|<span data-ttu-id="dd666-131">Обновление существующего trustFrameworkPolicy.</span><span class="sxs-lookup"><span data-stu-id="dd666-131">Update an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="dd666-132">Удаление trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="dd666-132">Delete trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-delete.md)|<span data-ttu-id="dd666-133">Нет</span><span class="sxs-lookup"><span data-stu-id="dd666-133">None</span></span>|<span data-ttu-id="dd666-134">Удаление существующего trustFrameworkPolicy.</span><span class="sxs-lookup"><span data-stu-id="dd666-134">Delete an existing trustFrameworkPolicy.</span></span>|

## <a name="properties"></a><span data-ttu-id="dd666-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd666-135">Properties</span></span>

|<span data-ttu-id="dd666-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd666-136">Property</span></span>|<span data-ttu-id="dd666-137">Тип</span><span class="sxs-lookup"><span data-stu-id="dd666-137">Type</span></span>|<span data-ttu-id="dd666-138">Описание</span><span class="sxs-lookup"><span data-stu-id="dd666-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd666-139">id</span><span class="sxs-lookup"><span data-stu-id="dd666-139">id</span></span>|<span data-ttu-id="dd666-140">String</span><span class="sxs-lookup"><span data-stu-id="dd666-140">String</span></span>|<span data-ttu-id="dd666-141">ID политики.</span><span class="sxs-lookup"><span data-stu-id="dd666-141">The ID of the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dd666-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd666-142">JSON representation</span></span>

<span data-ttu-id="dd666-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd666-143">The following is a JSON representation of the resource.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="dd666-144">См. также</span><span class="sxs-lookup"><span data-stu-id="dd666-144">See also</span></span>

- <span data-ttu-id="dd666-145">[схема trustFrameworkPolicy](/azure/active-directory-b2c/trustframeworkpolicy) для получения сведений о элементах схемы.</span><span class="sxs-lookup"><span data-stu-id="dd666-145">[trustFrameworkPolicy schema](/azure/active-directory-b2c/trustframeworkpolicy) for information about the schema elements.</span></span>
- [<span data-ttu-id="dd666-146">trustFrameworkPolicy.xsd</span><span class="sxs-lookup"><span data-stu-id="dd666-146">trustFrameworkPolicy.xsd</span></span>](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)


