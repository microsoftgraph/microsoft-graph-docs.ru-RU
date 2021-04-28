---
title: Создание открытого расширения
description: Создание открытого расширения (объекта openTypeExtension) и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.
localization_priority: Priority
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: f91a549e13b956d9c0d1fa4d8ca8765e7b7bd89a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052224"
---
# <a name="create-open-extension"></a><span data-ttu-id="e47ff-103">Создание открытого расширения</span><span class="sxs-lookup"><span data-stu-id="e47ff-103">Create open extension</span></span>

<span data-ttu-id="e47ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e47ff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e47ff-105">Создание открытого расширения (объекта [openTypeExtension](../resources/opentypeextension.md)) и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="e47ff-105">Create an open extension ([openTypeExtension](../resources/opentypeextension.md) object) and add custom properties in a new or existing instance of a resource.</span></span>

<span data-ttu-id="e47ff-106">В таблице раздела [Разрешения](#permissions) перечислены ресурсы, поддерживающие открытые расширения.</span><span class="sxs-lookup"><span data-stu-id="e47ff-106">The table in the [Permissions](#permissions) section lists the resources that support open extensions.</span></span>

> <span data-ttu-id="e47ff-107">**Примечание.** Если вы создаете открытые расширения для ресурсов Outlook, см. раздел **Рекомендации, касающиеся Outlook** в статье [Тип ресурса openTypeExtension](../resources/opentypeextension.md#outlook-specific-considerations).</span><span class="sxs-lookup"><span data-stu-id="e47ff-107">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="e47ff-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e47ff-108">Permissions</span></span>

<span data-ttu-id="e47ff-109">В зависимости от ресурса, в котором создается расширение, и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e47ff-109">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="e47ff-110">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e47ff-110">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e47ff-111">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="e47ff-111">Supported resource</span></span> | <span data-ttu-id="e47ff-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e47ff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e47ff-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e47ff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e47ff-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e47ff-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="e47ff-115">device</span><span class="sxs-lookup"><span data-stu-id="e47ff-115">device</span></span>](../resources/device.md) | <span data-ttu-id="e47ff-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e47ff-116">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="e47ff-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e47ff-117">Not supported</span></span> | <span data-ttu-id="e47ff-118">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e47ff-118">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="e47ff-119">event</span><span class="sxs-lookup"><span data-stu-id="e47ff-119">event</span></span>](../resources/event.md) | <span data-ttu-id="e47ff-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47ff-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="e47ff-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47ff-121">Calendars.ReadWrite</span></span> | <span data-ttu-id="e47ff-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47ff-122">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="e47ff-123">group</span><span class="sxs-lookup"><span data-stu-id="e47ff-123">group</span></span>](../resources/group.md) | <span data-ttu-id="e47ff-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e47ff-124">Group.ReadWrite.All</span></span> | <span data-ttu-id="e47ff-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e47ff-125">Not supported</span></span> | <span data-ttu-id="e47ff-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e47ff-126">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="e47ff-127">[event](../resources/event.md) для групп</span><span class="sxs-lookup"><span data-stu-id="e47ff-127">[group event](../resources/event.md)</span></span> | <span data-ttu-id="e47ff-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e47ff-128">Group.ReadWrite.All</span></span> | <span data-ttu-id="e47ff-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e47ff-129">Not supported</span></span> | <span data-ttu-id="e47ff-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e47ff-130">Not supported</span></span> |
| <span data-ttu-id="e47ff-131">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="e47ff-131">[group post](../resources/post.md)</span></span> | <span data-ttu-id="e47ff-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e47ff-132">Group.ReadWrite.All</span></span> | <span data-ttu-id="e47ff-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e47ff-133">Not supported</span></span> | <span data-ttu-id="e47ff-134">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e47ff-134">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="e47ff-135">message</span><span class="sxs-lookup"><span data-stu-id="e47ff-135">message</span></span>](../resources/message.md) | <span data-ttu-id="e47ff-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47ff-136">Mail.ReadWrite</span></span> | <span data-ttu-id="e47ff-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47ff-137">Mail.ReadWrite</span></span> | <span data-ttu-id="e47ff-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47ff-138">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="e47ff-139">organization</span><span class="sxs-lookup"><span data-stu-id="e47ff-139">organization</span></span>](../resources/organization.md) | <span data-ttu-id="e47ff-140">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e47ff-140">Organization.ReadWrite.All</span></span> | <span data-ttu-id="e47ff-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e47ff-141">Not supported</span></span> | <span data-ttu-id="e47ff-142">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e47ff-142">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="e47ff-143">[contact](../resources/contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="e47ff-143">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="e47ff-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47ff-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="e47ff-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47ff-145">Contacts.ReadWrite</span></span> | <span data-ttu-id="e47ff-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47ff-146">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="e47ff-147">user</span><span class="sxs-lookup"><span data-stu-id="e47ff-147">user</span></span>](../resources/user.md) | <span data-ttu-id="e47ff-148">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47ff-148">User.ReadWrite</span></span> | <span data-ttu-id="e47ff-149">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47ff-149">User.ReadWrite</span></span> | <span data-ttu-id="e47ff-150">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e47ff-150">User.ReadWrite.All</span></span> |
| [<span data-ttu-id="e47ff-151">task</span><span class="sxs-lookup"><span data-stu-id="e47ff-151">task</span></span>](../resources/todotask.md) | <span data-ttu-id="e47ff-152">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47ff-152">Tasks.ReadWrite</span></span> | <span data-ttu-id="e47ff-153">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47ff-153">Tasks.ReadWrite</span></span> | <span data-ttu-id="e47ff-154">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e47ff-154">Tasks.ReadWrite.All</span></span> |
| [<span data-ttu-id="e47ff-155">tasklist</span><span class="sxs-lookup"><span data-stu-id="e47ff-155">tasklist</span></span>](../resources/todotasklist.md)  | <span data-ttu-id="e47ff-156">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47ff-156">Tasks.ReadWrite</span></span> | <span data-ttu-id="e47ff-157">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e47ff-157">Tasks.ReadWrite</span></span> | <span data-ttu-id="e47ff-158">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e47ff-158">Tasks.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e47ff-159">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e47ff-159">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="e47ff-160">Создание расширения в новом экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="e47ff-160">Create an extension in a new resource instance</span></span>

<span data-ttu-id="e47ff-161">Используйте такой же запрос REST, как для создания экземпляра.</span><span class="sxs-lookup"><span data-stu-id="e47ff-161">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
POST /users/{id|userPrincipalName}/todo/lists/{id}/tasks
POST /users/{id|userPrincipalName}/todo/lists
```

><span data-ttu-id="e47ff-162">**Примечание.** В этом синтаксисе показаны некоторые распространенные способы создания поддерживаемых экземпляров ресурса.</span><span class="sxs-lookup"><span data-stu-id="e47ff-162">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="e47ff-163">Все другие варианты синтаксиса POST, позволяющие создавать эти экземпляры ресурса, поддерживают создание открытых расширений этих экземпляров подобным образом.</span><span class="sxs-lookup"><span data-stu-id="e47ff-163">All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="e47ff-164">В разделе [Текст запроса](#request-body) показано, как включить свойства нового экземпляра ресурса _и расширение_ в текст запроса.</span><span class="sxs-lookup"><span data-stu-id="e47ff-164">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="e47ff-165">Создание расширения в существующем экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="e47ff-165">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="e47ff-166">Идентифицируйте экземпляр ресурса в запросе и выполните операцию `POST` для свойства навигации **extensions**.</span><span class="sxs-lookup"><span data-stu-id="e47ff-166">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/extensions
POST /users/{id|userPrincipalName}/events/{id}/extensions
POST /groups/{id}/extensions
POST /groups/{id}/events/{id}/extensions
POST /groups/{id}/threads/{id}/posts/{id}/extensions
POST /users/{id|userPrincipalName}/messages/{id}/extensions
POST /organization/{id}/extensions
POST /users/{id|userPrincipalName}/contacts/{id}/extensions
POST /users/{id|userPrincipalName}/extensions
POST /users/{id|userPrincipalName}/todo/lists/{id}/tasks/{id}/extensions
POST /users/{id|userPrincipalName}/todo/lists/{id}/extensions
```

><span data-ttu-id="e47ff-p103">**Примечание.** В этом синтаксисе показаны некоторые распространенные способы определения экземпляра ресурса, чье расширение нужно удалить. Все другие варианты синтаксиса, позволяющие определить эти экземпляры ресурса, поддерживают удаление открытых расширений этих экземпляров подобным образом.</span><span class="sxs-lookup"><span data-stu-id="e47ff-p103">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it. All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="e47ff-169">В разделе [Текст запроса](#request-body) показано, как включить _расширение_ в текст запроса.</span><span class="sxs-lookup"><span data-stu-id="e47ff-169">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="e47ff-170">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="e47ff-170">Path parameters</span></span>
|<span data-ttu-id="e47ff-171">Параметр</span><span class="sxs-lookup"><span data-stu-id="e47ff-171">Parameter</span></span>|<span data-ttu-id="e47ff-172">Тип</span><span class="sxs-lookup"><span data-stu-id="e47ff-172">Type</span></span>|<span data-ttu-id="e47ff-173">Описание</span><span class="sxs-lookup"><span data-stu-id="e47ff-173">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e47ff-174">id</span><span class="sxs-lookup"><span data-stu-id="e47ff-174">id</span></span>|<span data-ttu-id="e47ff-175">string</span><span class="sxs-lookup"><span data-stu-id="e47ff-175">string</span></span>|<span data-ttu-id="e47ff-p104">Уникальный идентификатор объекта в соответствующей коллекции. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e47ff-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e47ff-178">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e47ff-178">Request headers</span></span>

| <span data-ttu-id="e47ff-179">Имя</span><span class="sxs-lookup"><span data-stu-id="e47ff-179">Name</span></span>       | <span data-ttu-id="e47ff-180">Значение</span><span class="sxs-lookup"><span data-stu-id="e47ff-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e47ff-181">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e47ff-181">Authorization</span></span> | <span data-ttu-id="e47ff-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e47ff-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e47ff-184">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e47ff-184">Content-Type</span></span> | <span data-ttu-id="e47ff-185">application/json</span><span class="sxs-lookup"><span data-stu-id="e47ff-185">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e47ff-186">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e47ff-186">Request body</span></span>

<span data-ttu-id="e47ff-p106">Предоставьте описание объекта [openTypeExtension](../resources/opentypeextension.md) в формате JSON с указанными ниже обязательными парами "имя-значение", а также дополнительными пользовательскими данными. Полезные данные JSON могут относиться к простому типу или представлять собой массив элементов простого типа.</span><span class="sxs-lookup"><span data-stu-id="e47ff-p106">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs, and any additional custom data. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="e47ff-189">Имя</span><span class="sxs-lookup"><span data-stu-id="e47ff-189">Name</span></span>       | <span data-ttu-id="e47ff-190">Значение</span><span class="sxs-lookup"><span data-stu-id="e47ff-190">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e47ff-191">@odata.type</span><span class="sxs-lookup"><span data-stu-id="e47ff-191">@odata.type</span></span> | <span data-ttu-id="e47ff-192">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="e47ff-192">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="e47ff-193">extensionName</span><span class="sxs-lookup"><span data-stu-id="e47ff-193">extensionName</span></span> | <span data-ttu-id="e47ff-194">%уникальная_строка%</span><span class="sxs-lookup"><span data-stu-id="e47ff-194">%unique_string%</span></span> |

<span data-ttu-id="e47ff-195">При создании расширения в _новом_ экземпляре ресурса предоставьте не только объект **openTypeExtension**, но и представление JSON соответствующих свойств для создания этого экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="e47ff-195">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="e47ff-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="e47ff-196">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="e47ff-197">Код ответа</span><span class="sxs-lookup"><span data-stu-id="e47ff-197">Response code</span></span>

<span data-ttu-id="e47ff-198">В зависимости от операции можно использовать код ответа `201 Created` или `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="e47ff-198">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="e47ff-p107">При создании расширения с использованием такой же операции, как для создания экземпляра ресурса, операция возвращает такой же код отклика, что и при создании экземпляра ресурса без расширения. Изучите соответствующие статьи о создании экземпляров, перечисленные [выше](#create-an-extension-in-a-new-resource-instance).</span><span class="sxs-lookup"><span data-stu-id="e47ff-p107">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension. Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="e47ff-201">Текст отклика</span><span class="sxs-lookup"><span data-stu-id="e47ff-201">Response body</span></span>

| <span data-ttu-id="e47ff-202">Сценарий</span><span class="sxs-lookup"><span data-stu-id="e47ff-202">Scenario</span></span>       | <span data-ttu-id="e47ff-203">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e47ff-203">Resource</span></span>  | <span data-ttu-id="e47ff-204">Текст отклика</span><span class="sxs-lookup"><span data-stu-id="e47ff-204">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="e47ff-205">Создание расширения с явным созданием _нового_ экземпляра ресурса</span><span class="sxs-lookup"><span data-stu-id="e47ff-205">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="e47ff-206">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="e47ff-206">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="e47ff-207">Включает новый экземпляр, дополненный объектом [openTypeExtension](../resources/opentypeextension.md).</span><span class="sxs-lookup"><span data-stu-id="e47ff-207">Includes the new instance expanded with the [openTypeExtension](../resources/opentypeextension.md) object.</span></span> |
| <span data-ttu-id="e47ff-208">Создание расширения с неявным созданием экземпляра ресурса</span><span class="sxs-lookup"><span data-stu-id="e47ff-208">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="e47ff-209">post</span><span class="sxs-lookup"><span data-stu-id="e47ff-209">post</span></span>](../resources/post.md) | <span data-ttu-id="e47ff-210">Ответ содержит только код ответа без текста.</span><span class="sxs-lookup"><span data-stu-id="e47ff-210">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="e47ff-211">Создание расширения в _существующем_ экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="e47ff-211">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="e47ff-212">Все поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="e47ff-212">All supported resources</span></span> | <span data-ttu-id="e47ff-213">Включает объект **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="e47ff-213">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="e47ff-214">Пример</span><span class="sxs-lookup"><span data-stu-id="e47ff-214">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="e47ff-215">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="e47ff-215">Request 1</span></span>

<span data-ttu-id="e47ff-p108">В первом примере сообщение и расширение создаются в одном запросе. Текст запроса включает следующие данные:</span><span class="sxs-lookup"><span data-stu-id="e47ff-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="e47ff-218">Свойства **subject**, **body** и **toRecipients**, характерные для нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="e47ff-218">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="e47ff-219">Данные для расширения:</span><span class="sxs-lookup"><span data-stu-id="e47ff-219">And for the extension:</span></span>

  - <span data-ttu-id="e47ff-220">Тип `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="e47ff-220">The type `microsoft.graph.openTypeExtension`.</span></span>
  - <span data-ttu-id="e47ff-221">Имя расширения "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="e47ff-221">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="e47ff-222">Дополнительные данные, хранящиеся в виде трех настраиваемых свойств в полезных данных JSON: `companyName`, `expirationDate` и `dealValue`.</span><span class="sxs-lookup"><span data-stu-id="e47ff-222">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>


# <a name="http"></a>[<span data-ttu-id="e47ff-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="e47ff-223">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages

{
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "You should be proud!"
  },
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com"
      }
    }
  ],
  "extensions": [
    {
      "@odata.type": "microsoft.graph.openTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="e47ff-224">C#</span><span class="sxs-lookup"><span data-stu-id="e47ff-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e47ff-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e47ff-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e47ff-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e47ff-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-1"></a><span data-ttu-id="e47ff-227">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="e47ff-227">Response 1</span></span>

<span data-ttu-id="e47ff-p109">Ниже представлен отклик для первого примера. Текст отклика включает свойства нового сообщения и следующие данные для нового расширения:</span><span class="sxs-lookup"><span data-stu-id="e47ff-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="e47ff-230">Свойство **id** с полным именем `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="e47ff-230">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="e47ff-231">Стандартное свойство **extensionName**, указанное в запросе.</span><span class="sxs-lookup"><span data-stu-id="e47ff-231">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="e47ff-232">Пользовательские данные из запроса, сохраненные в виде 3 настраиваемых свойств.</span><span class="sxs-lookup"><span data-stu-id="e47ff-232">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="e47ff-233">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e47ff-233">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')",
  "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj\"",
  "id": "AAMkAGEbs88AAB84uLuAAA=",
  "createdDateTime": "2015-10-30T03:03:43Z",
  "lastModifiedDateTime": "2015-10-30T03:03:43Z",
  "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj",
  "categories": [ ],
  "receivedDateTime": "2015-10-30T03:03:43Z",
  "sentDateTime": "2015-10-30T03:03:43Z",
  "hasAttachments": false,
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r
\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nYou should be proud!\r\n</body>\r
\n</html>\r\n"
  },
  "bodyPreview": "You should be proud!",
  "importance": "Normal",
  "parentFolderId": "AQMkAGEwAAAIBDwAAAA==",
  "sender": null,
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com",
        "name": "John Doe"
      }
    }
  ],
  "ccRecipients": [ ],
  "bccRecipients": [ ],
  "replyTo": [ ],
  "conversationId": "AAQkAGEFGugh3SVdMzzc=",
  "isDeliveryReceiptRequested": false,
  "isReadReceiptRequested": false,
  "isRead": true,
  "isDraft": true,
  "webLink": "https://outlook.office.com/owa/?
ItemID=AAMkAGEbs88AAB84uLuAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
  "inferenceClassification": "Focused",
  "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages
('AAMkAGEbs88AAB84uLuAAA%3D')/extensions",
  "extensions": [
    {
      "@odata.type": "#microsoft.graph.openTypeExtension",
      "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('microsoft.graph.openTypeExtension.Com.Contoso.Referral')",
      "id": "microsoft.graph.openTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

****

### <a name="request-2"></a><span data-ttu-id="e47ff-234">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="e47ff-234">Request 2</span></span>

<span data-ttu-id="e47ff-p110">Во втором примере показано создание расширения в указанном сообщении. Текст запроса включает следующие данные для расширения:</span><span class="sxs-lookup"><span data-stu-id="e47ff-p110">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="e47ff-237">Тип `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="e47ff-237">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="e47ff-238">Имя расширения "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="e47ff-238">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="e47ff-239">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `dealValue` и `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="e47ff-239">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>


# <a name="http"></a>[<span data-ttu-id="e47ff-240">HTTP</span><span class="sxs-lookup"><span data-stu-id="e47ff-240">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```
# <a name="c"></a>[<span data-ttu-id="e47ff-241">C#</span><span class="sxs-lookup"><span data-stu-id="e47ff-241">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e47ff-242">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e47ff-242">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e47ff-243">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e47ff-243">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-2"></a><span data-ttu-id="e47ff-244">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="e47ff-244">Response 2</span></span>

<span data-ttu-id="e47ff-p111">Ниже представлен отклик для второго примера. Текст отклика включает следующие данные для нового расширения:</span><span class="sxs-lookup"><span data-stu-id="e47ff-p111">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="e47ff-247">Свойство по умолчанию **extensionName**.</span><span class="sxs-lookup"><span data-stu-id="e47ff-247">The default property **extensionName**.</span></span>
- <span data-ttu-id="e47ff-248">Свойство **id** с полным именем `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="e47ff-248">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="e47ff-249">Сохраняемые пользовательские данные.</span><span class="sxs-lookup"><span data-stu-id="e47ff-249">The custom data to be stored.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('microsoft.graph.openTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "microsoft.graph.openTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

### <a name="request-3"></a><span data-ttu-id="e47ff-250">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="e47ff-250">Request 3</span></span>

<span data-ttu-id="e47ff-p112">В третьем примере показано создание расширения в указанном событии группы. Текст запроса включает следующие данные для расширения:</span><span class="sxs-lookup"><span data-stu-id="e47ff-p112">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="e47ff-253">Тип `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="e47ff-253">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="e47ff-254">Имя расширения "Com.Contoso.Deal".</span><span class="sxs-lookup"><span data-stu-id="e47ff-254">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="e47ff-255">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `dealValue` и `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="e47ff-255">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>


# <a name="http"></a>[<span data-ttu-id="e47ff-256">HTTP</span><span class="sxs-lookup"><span data-stu-id="e47ff-256">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```
# <a name="c"></a>[<span data-ttu-id="e47ff-257">C#</span><span class="sxs-lookup"><span data-stu-id="e47ff-257">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e47ff-258">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e47ff-258">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e47ff-259">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e47ff-259">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-3"></a><span data-ttu-id="e47ff-260">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="e47ff-260">Response 3</span></span>

<span data-ttu-id="e47ff-261">Ниже представлен отклик из третьего примера.</span><span class="sxs-lookup"><span data-stu-id="e47ff-261">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "microsoft.graph.openTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

### <a name="request-4"></a><span data-ttu-id="e47ff-262">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="e47ff-262">Request 4</span></span>

<span data-ttu-id="e47ff-p113">В четвертом примере показано создание расширения в новой записи группы с помощью одного вызова действия **reply** для существующей записи группы. Действие **reply** создает запись и внедряет в нее новое расширение. Текст запроса включает свойство **post**, которое, в свою очередь, содержит свойство **body** новой записи и следующие данные для нового расширения:</span><span class="sxs-lookup"><span data-stu-id="e47ff-p113">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="e47ff-266">Тип `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="e47ff-266">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="e47ff-267">Имя расширения "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="e47ff-267">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="e47ff-268">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `expirationDate` и массив строк `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="e47ff-268">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>


# <a name="http"></a>[<span data-ttu-id="e47ff-269">HTTP</span><span class="sxs-lookup"><span data-stu-id="e47ff-269">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=/reply

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "microsoft.graph.openTypeExtension",
      "extensionName": "Com.Contoso.HR",
      "companyName": "Contoso",
      "expirationDate": "2015-07-03T13:04:00.000Z",
      "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
      ]
    }
  ]
  }
}
```
# <a name="c"></a>[<span data-ttu-id="e47ff-270">C#</span><span class="sxs-lookup"><span data-stu-id="e47ff-270">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e47ff-271">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e47ff-271">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e47ff-272">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e47ff-272">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-4"></a><span data-ttu-id="e47ff-273">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="e47ff-273">Response 4</span></span>

<span data-ttu-id="e47ff-p114">Ниже представлен отклик из четвертого примера. При успешном создании расширения в новой записи группы возвращается только код отклика HTTP 202.</span><span class="sxs-lookup"><span data-stu-id="e47ff-p114">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Content-type: text/plain
Content-Length: 0
```

****

### <a name="request-5"></a><span data-ttu-id="e47ff-276">Запрос 5</span><span class="sxs-lookup"><span data-stu-id="e47ff-276">Request 5</span></span>

<span data-ttu-id="e47ff-p115">В пятом примере показано создание расширения в новой записи группы с помощью той же операции POST, которая создает беседу. Операция POST создает беседу, цепочку и запись, а также внедряет в эту запись новое расширение. Текст отклика включает свойства **Topic** и **Threads**, а также дочерний объект **post** для новой беседы. Объект **post**, в свою очередь, содержит свойство **body** новой записи и следующие данные расширения:</span><span class="sxs-lookup"><span data-stu-id="e47ff-p115">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="e47ff-281">Тип `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="e47ff-281">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="e47ff-282">Имя расширения "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="e47ff-282">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="e47ff-283">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `expirationDate` и массив строк `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="e47ff-283">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>


# <a name="http"></a>[<span data-ttu-id="e47ff-284">HTTP</span><span class="sxs-lookup"><span data-stu-id="e47ff-284">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/conversations

{
  "Topic": "Does anyone have a second?",
  "Threads": [
    {
      "Posts": [
        {
          "Body": {
            "ContentType": "HTML",
            "Content": "This is urgent!"
          },
          "Extensions": [
            {
              "@odata.type": "microsoft.graph.openTypeExtension",
              "extensionName": "Com.Contoso.Benefits",
              "companyName": "Contoso",
              "expirationDate": "2016-08-03T11:00:00.000Z",
              "topPicks": [
                "Employees only",
                "Add spouse or guest",
                "Add family"
              ]
            }
          ]
        }
      ]
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="e47ff-285">C#</span><span class="sxs-lookup"><span data-stu-id="e47ff-285">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e47ff-286">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e47ff-286">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e47ff-287">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e47ff-287">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-5"></a><span data-ttu-id="e47ff-288">Отклик 5</span><span class="sxs-lookup"><span data-stu-id="e47ff-288">Response 5</span></span>

<span data-ttu-id="e47ff-p116">Ниже представлен отклик из пятого примера, содержащий новую беседу и идентификатор цепочки. Эта новая цепочка содержит автоматически созданную запись, включающую новое расширение.</span><span class="sxs-lookup"><span data-stu-id="e47ff-p116">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="e47ff-291">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e47ff-291">Note: The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="e47ff-p117">Чтобы получить новое расширение, сначала [получите все записи](../api/conversationthread-list-posts.md) из цепочки. Изначально в ней должна быть только одна запись. Затем примените идентификатор записи и имя расширения `Com.Contoso.Benefits`, чтобы [получить расширение](../api/opentypeextension-get.md).</span><span class="sxs-lookup"><span data-stu-id="e47ff-p117">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
    "threads": [
        {
            "id": "AAQkADJDtMUzsf_PdhAAswJOhGVsnkyDtMUzsf_Pdg=="
        }
    ]
}

```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

