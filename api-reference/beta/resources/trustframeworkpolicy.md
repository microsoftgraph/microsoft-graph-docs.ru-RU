---
title: Трустфрамеворкполици
description: В политике Azure AD B2C Trust Framework называются пользовательскими политиками. В этом разделе описываются операции, доступные в объекте Трустфрамеворкполици для клиента.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8b822f1b9788d0502c1376ed437593dfb96469ad
ms.sourcegitcommit: d264fa064215879fa88a4680402cd57a470d73db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2019
ms.locfileid: "31989396"
---
# <a name="trustframeworkpolicy-resource-type"></a><span data-ttu-id="7d58e-104">Тип ресурса Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="7d58e-104">trustFrameworkPolicy resource type</span></span>

> <span data-ttu-id="7d58e-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7d58e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d58e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d58e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d58e-107">Представляет политику [платформы доверия](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) (также называемую [настраиваемой политикой](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom)) в [Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview).</span><span class="sxs-lookup"><span data-stu-id="7d58e-107">Represents a [Trust Framework](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) policy (also called [custom policy](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom)) in [Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview).</span></span> <span data-ttu-id="7d58e-108">Политика инфраструктуры доверия предоставляет полный контроль над путешествием пользователей.</span><span class="sxs-lookup"><span data-stu-id="7d58e-108">A Trust Framework policy gives full control over the user journeys.</span></span> <span data-ttu-id="7d58e-109">Используйте его для:</span><span class="sxs-lookup"><span data-stu-id="7d58e-109">Use it to:</span></span>

* <span data-ttu-id="7d58e-110">Полностью настройте вход и вход в систему.</span><span class="sxs-lookup"><span data-stu-id="7d58e-110">Customize the sign-up and sign-in experiences fully.</span></span>
* <span data-ttu-id="7d58e-111">Федерацию на любой поставщик удостоверений SAML, Open ID Connect или OAuth2.</span><span class="sxs-lookup"><span data-stu-id="7d58e-111">Federate to any SAML, Open ID Connect, or OAuth2 identity provider.</span></span>
* <span data-ttu-id="7d58e-112">Интеграция с другими системами или хранилищами пользовательских данных путем вызова конечных точек REST.</span><span class="sxs-lookup"><span data-stu-id="7d58e-112">Integrate with other systems or user data stores by calling REST endpoints.</span></span>
* <span data-ttu-id="7d58e-113">Преобразование утверждений и настройка маркеров, выданных приложению проверяющей стороны.</span><span class="sxs-lookup"><span data-stu-id="7d58e-113">Transform claims and customize tokens issued to the relying party application.</span></span>

<span data-ttu-id="7d58e-114">Для получения дополнительных сведений см. [настраиваемые политики в Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span><span class="sxs-lookup"><span data-stu-id="7d58e-114">For more information, see [Custom policies in Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span></span>

## <a name="methods"></a><span data-ttu-id="7d58e-115">Методы</span><span class="sxs-lookup"><span data-stu-id="7d58e-115">Methods</span></span>

| <span data-ttu-id="7d58e-116">Метод</span><span class="sxs-lookup"><span data-stu-id="7d58e-116">Method</span></span>       | <span data-ttu-id="7d58e-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7d58e-117">Return Type</span></span>  |<span data-ttu-id="7d58e-118">Описание</span><span class="sxs-lookup"><span data-stu-id="7d58e-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7d58e-119">Создание Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="7d58e-119">Create trustFrameworkPolicy</span></span>](../api/trustframework-post-trustframeworkpolicy.md)|<span data-ttu-id="7d58e-120">Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="7d58e-120">trustFrameworkPolicy</span></span>|<span data-ttu-id="7d58e-121">Создание нового Трустфрамеворкполици.</span><span class="sxs-lookup"><span data-stu-id="7d58e-121">Create a new trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="7d58e-122">Получение Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="7d58e-122">Get trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-get.md) |<span data-ttu-id="7d58e-123">Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="7d58e-123">trustFrameworkPolicy</span></span>|<span data-ttu-id="7d58e-124">Чтение свойств существующего Трустфрамеворкполици.</span><span class="sxs-lookup"><span data-stu-id="7d58e-124">Read properties of an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="7d58e-125">Список ТрустфрамеворкполиЦиес</span><span class="sxs-lookup"><span data-stu-id="7d58e-125">List trustFrameworkPolicies</span></span>](../api/trustframework-list-trustframeworkpolicies.md)|<span data-ttu-id="7d58e-126">Коллекция Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="7d58e-126">trustFrameworkPolicy collection</span></span>|<span data-ttu-id="7d58e-127">Список всех ТрустфрамеворкполиЦиес, настроенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="7d58e-127">List all trustFrameworkPolicies configured in a tenant.</span></span>|
|[<span data-ttu-id="7d58e-128">Обновление или создание Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="7d58e-128">Update or create trustFrameworkPolicy</span></span>](../api/trustframework-put-trustframeworkpolicy.md)|<span data-ttu-id="7d58e-129">Нет</span><span class="sxs-lookup"><span data-stu-id="7d58e-129">None</span></span>|<span data-ttu-id="7d58e-130">Обновление существующего Трустфрамеворкполици.</span><span class="sxs-lookup"><span data-stu-id="7d58e-130">Update an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="7d58e-131">Удаление Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="7d58e-131">Delete trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-delete.md)|<span data-ttu-id="7d58e-132">Нет</span><span class="sxs-lookup"><span data-stu-id="7d58e-132">None</span></span>|<span data-ttu-id="7d58e-133">Удаление существующего Трустфрамеворкполици.</span><span class="sxs-lookup"><span data-stu-id="7d58e-133">Delete an existing trustFrameworkPolicy.</span></span>|

## <a name="properties"></a><span data-ttu-id="7d58e-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d58e-134">Properties</span></span>

|<span data-ttu-id="7d58e-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d58e-135">Property</span></span>|<span data-ttu-id="7d58e-136">Тип</span><span class="sxs-lookup"><span data-stu-id="7d58e-136">Type</span></span>|<span data-ttu-id="7d58e-137">Описание</span><span class="sxs-lookup"><span data-stu-id="7d58e-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d58e-138">id</span><span class="sxs-lookup"><span data-stu-id="7d58e-138">id</span></span>|<span data-ttu-id="7d58e-139">Строка</span><span class="sxs-lookup"><span data-stu-id="7d58e-139">String</span></span>|<span data-ttu-id="7d58e-140">Идентификатор политики.</span><span class="sxs-lookup"><span data-stu-id="7d58e-140">The ID of the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d58e-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d58e-141">JSON representation</span></span>

<span data-ttu-id="7d58e-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d58e-142">The following is a JSON representation of the resource.</span></span>

```json
{
   "id": "B2C_1A_Test"
}
```

## <a name="see-also"></a><span data-ttu-id="7d58e-143">См. также</span><span class="sxs-lookup"><span data-stu-id="7d58e-143">See also</span></span>

- <span data-ttu-id="7d58e-144">[схема трустфрамеворкполици](https://docs.microsoft.com/en-us/azure/active-directory-b2c/trustframeworkpolicy) для получения сведений об элементах схемы.</span><span class="sxs-lookup"><span data-stu-id="7d58e-144">[trustFrameworkPolicy schema](https://docs.microsoft.com/en-us/azure/active-directory-b2c/trustframeworkpolicy) for information about the schema elements.</span></span>  
- [<span data-ttu-id="7d58e-145">Трустфрамеворкполици. xsd</span><span class="sxs-lookup"><span data-stu-id="7d58e-145">trustFrameworkPolicy.xsd</span></span>](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)
