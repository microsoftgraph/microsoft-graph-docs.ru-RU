---
title: Создание открытого расширения
description: Создание расширения open (объект openTypeExtension) и Добавление настраиваемых свойств
ms.openlocfilehash: 80747559d310f033419fe3b24add1dc27debb90e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079107"
---
# <a name="create-open-extension"></a><span data-ttu-id="79b49-103">Создание открытого расширения</span><span class="sxs-lookup"><span data-stu-id="79b49-103">Create open extension</span></span>

> <span data-ttu-id="79b49-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="79b49-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79b49-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79b49-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79b49-106">Создайте расширение open (объект[openTypeExtension](../resources/opentypeextension.md) ) и добавьте настраиваемых свойств в новый или существующий экземпляр поддерживаемые ресурсов.</span><span class="sxs-lookup"><span data-stu-id="79b49-106">Create an open extension ([openTypeExtension](../resources/opentypeextension.md) object) and add custom properties in a new or existing instance of a supported resource.</span></span>

> <span data-ttu-id="79b49-107">**Примечание:** При создании open расширения Outlook ресурсов, содержатся в разделе **относящиеся к Outlook** в разделе [Тип ресурса openTypeExtension](../resources/opentypeextension.md#outlook-specific-considerations).</span><span class="sxs-lookup"><span data-stu-id="79b49-107">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="79b49-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="79b49-108">Permissions</span></span>

<span data-ttu-id="79b49-109">В зависимости от разрешений и ресурсов, которое вы создаете расширения в тип (делегированные или приложение) запрошенный, разрешение, указанное в следующей таблице минимальными правами требуется для вызова этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="79b49-109">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="79b49-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79b49-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79b49-111">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="79b49-111">Supported resource</span></span> | <span data-ttu-id="79b49-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79b49-112">Delegated (work or school account)</span></span> | <span data-ttu-id="79b49-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79b49-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79b49-114">Для приложения</span><span class="sxs-lookup"><span data-stu-id="79b49-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="79b49-115">device</span><span class="sxs-lookup"><span data-stu-id="79b49-115">device</span></span>](../resources/device.md) | <span data-ttu-id="79b49-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="79b49-116">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="79b49-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="79b49-117">Not supported</span></span> | <span data-ttu-id="79b49-118">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79b49-118">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="79b49-119">event</span><span class="sxs-lookup"><span data-stu-id="79b49-119">event</span></span>](../resources/event.md) | <span data-ttu-id="79b49-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79b49-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="79b49-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79b49-121">Calendars.ReadWrite</span></span> | <span data-ttu-id="79b49-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79b49-122">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="79b49-123">group</span><span class="sxs-lookup"><span data-stu-id="79b49-123">group</span></span>](../resources/group.md) | <span data-ttu-id="79b49-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79b49-124">Group.ReadWrite.All</span></span> | <span data-ttu-id="79b49-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="79b49-125">Not supported</span></span> | <span data-ttu-id="79b49-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79b49-126">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="79b49-127">[event](../resources/event.md) для групп</span><span class="sxs-lookup"><span data-stu-id="79b49-127">[group event](../resources/event.md)</span></span> | <span data-ttu-id="79b49-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79b49-128">Group.ReadWrite.All</span></span> | <span data-ttu-id="79b49-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="79b49-129">Not supported</span></span> | <span data-ttu-id="79b49-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="79b49-130">Not supported</span></span> |
| <span data-ttu-id="79b49-131">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="79b49-131">[group post](../resources/post.md)</span></span> | <span data-ttu-id="79b49-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79b49-132">Group.ReadWrite.All</span></span> | <span data-ttu-id="79b49-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="79b49-133">Not supported</span></span> | <span data-ttu-id="79b49-134">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79b49-134">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="79b49-135">message</span><span class="sxs-lookup"><span data-stu-id="79b49-135">message</span></span>](../resources/message.md) | <span data-ttu-id="79b49-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79b49-136">Mail.ReadWrite</span></span> | <span data-ttu-id="79b49-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79b49-137">Mail.ReadWrite</span></span> | <span data-ttu-id="79b49-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79b49-138">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="79b49-139">organization</span><span class="sxs-lookup"><span data-stu-id="79b49-139">organization</span></span>](../resources/organization.md) | <span data-ttu-id="79b49-140">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="79b49-140">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="79b49-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="79b49-141">Not supported</span></span> | <span data-ttu-id="79b49-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="79b49-142">Not supported</span></span> |
| <span data-ttu-id="79b49-143">[contact](../resources/contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="79b49-143">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="79b49-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79b49-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="79b49-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79b49-145">Contacts.ReadWrite</span></span> | <span data-ttu-id="79b49-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79b49-146">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="79b49-147">user</span><span class="sxs-lookup"><span data-stu-id="79b49-147">user</span></span>](../resources/user.md) | <span data-ttu-id="79b49-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79b49-148">User.ReadWrite.All</span></span> | <span data-ttu-id="79b49-149">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79b49-149">User.ReadWrite</span></span> | <span data-ttu-id="79b49-150">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79b49-150">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79b49-151">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79b49-151">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="79b49-152">Создание расширения в новом экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="79b49-152">Create an extension in a new resource instance</span></span>

<span data-ttu-id="79b49-153">Использование того же запроса REST, которая используется для создания экземпляра.</span><span class="sxs-lookup"><span data-stu-id="79b49-153">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="79b49-154">**Примечание:** Этот синтаксис показаны наиболее распространенные способы создания экземпляров поддерживаемые ресурсов.</span><span class="sxs-lookup"><span data-stu-id="79b49-154">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="79b49-155">Все синтаксис POST, которые можно создавать экземпляры этих ресурсов поддерживает создание open расширения в их аналогичным образом.</span><span class="sxs-lookup"><span data-stu-id="79b49-155">All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="79b49-156">В разделе [Тело запроса](#request-body) показано, как включить свойства нового экземпляра ресурса _и расширение_ в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="79b49-156">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="79b49-157">Создание расширения в существующем экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="79b49-157">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="79b49-158">Идентифицируйте экземпляр ресурса в запросе и выполните операцию `POST` для свойства навигации **extensions**.</span><span class="sxs-lookup"><span data-stu-id="79b49-158">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /administrativeunits/{id}/extensions
POST /devices/{id}/extensions
POST /users/{id|userPrincipalName}/events/{id}/extensions
POST /groups/{id}/extensions
POST /groups/{id}/events/{id}/extensions
POST /groups/{id}/threads/{id}/posts/{id}/extensions
POST /users/{id|userPrincipalName}/messages/{id}/extensions
POST /organization/{id}/extensions
POST /users/{id|userPrincipalName}/contacts/{id}/extensions
POST /users/{id|userPrincipalName}/extensions
```

><span data-ttu-id="79b49-159">**Примечание:** Этот синтаксис показаны наиболее распространенные способы идентификации экземпляра ресурсов, чтобы создать расширение в его.</span><span class="sxs-lookup"><span data-stu-id="79b49-159">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it.</span></span> <span data-ttu-id="79b49-160">Все другие синтаксисы, позволяет легко идентифицировать экземпляры этих ресурсов поддерживает создание open расширений в их аналогичным образом.</span><span class="sxs-lookup"><span data-stu-id="79b49-160">All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="79b49-161">В разделе [Тело запроса](#request-body) показано, как включить _расширение_ в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="79b49-161">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="79b49-162">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="79b49-162">Path parameters</span></span>

|<span data-ttu-id="79b49-163">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="79b49-163">**Parameter**</span></span>|<span data-ttu-id="79b49-164">**Тип**</span><span class="sxs-lookup"><span data-stu-id="79b49-164">**Type**</span></span>|<span data-ttu-id="79b49-165">**Описание**</span><span class="sxs-lookup"><span data-stu-id="79b49-165">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="79b49-166">id</span><span class="sxs-lookup"><span data-stu-id="79b49-166">id</span></span>|<span data-ttu-id="79b49-167">строка</span><span class="sxs-lookup"><span data-stu-id="79b49-167">string</span></span>|<span data-ttu-id="79b49-p105">Уникальный идентификатор объекта в соответствующей коллекции. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79b49-p105">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="79b49-170">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79b49-170">Request headers</span></span>

| <span data-ttu-id="79b49-171">Имя</span><span class="sxs-lookup"><span data-stu-id="79b49-171">Name</span></span>       | <span data-ttu-id="79b49-172">Значение</span><span class="sxs-lookup"><span data-stu-id="79b49-172">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="79b49-173">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79b49-173">Authorization</span></span> | <span data-ttu-id="79b49-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79b49-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79b49-176">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79b49-176">Content-Type</span></span> | <span data-ttu-id="79b49-177">application/json</span><span class="sxs-lookup"><span data-stu-id="79b49-177">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="79b49-178">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79b49-178">Request body</span></span>

<span data-ttu-id="79b49-179">Предоставьте JSON в тексте [openTypeExtension](../resources/opentypeextension.md)следующие обязательные пар имя значение и любые дополнительные пользовательские данные.</span><span class="sxs-lookup"><span data-stu-id="79b49-179">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs and any additional custom data.</span></span> <span data-ttu-id="79b49-180">JSON полезных данных может быть простых типов или массивами простых типов.</span><span class="sxs-lookup"><span data-stu-id="79b49-180">The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="79b49-181">Имя</span><span class="sxs-lookup"><span data-stu-id="79b49-181">Name</span></span>       | <span data-ttu-id="79b49-182">Значение</span><span class="sxs-lookup"><span data-stu-id="79b49-182">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="79b49-183">@odata.type</span><span class="sxs-lookup"><span data-stu-id="79b49-183">@odata.type</span></span> | <span data-ttu-id="79b49-184">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="79b49-184">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="79b49-185">extensionName</span><span class="sxs-lookup"><span data-stu-id="79b49-185">extensionName</span></span> | <span data-ttu-id="79b49-186">%уникальная_строка%</span><span class="sxs-lookup"><span data-stu-id="79b49-186">%unique_string%</span></span> |

<span data-ttu-id="79b49-187">При создании расширения в _новом_ экземпляре ресурса предоставьте не только объект **openTypeExtension**, но и представление JSON соответствующих свойств для создания этого экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="79b49-187">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="79b49-188">Ответ</span><span class="sxs-lookup"><span data-stu-id="79b49-188">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="79b49-189">Код ответа</span><span class="sxs-lookup"><span data-stu-id="79b49-189">Response code</span></span>

<span data-ttu-id="79b49-190">В зависимости от операции, можно использовать код ответа `201 Created` или `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="79b49-190">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="79b49-191">При создании расширения с помощью той же операции, которая используется для создания экземпляра ресурсов, операция возвращает один и тот же код ответа, который возвращается при использовании операции для создания экземпляра ресурсов без расширения.</span><span class="sxs-lookup"><span data-stu-id="79b49-191">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension.</span></span>
<span data-ttu-id="79b49-192">Ссылки на соответствующие разделы для создания экземпляра как перечисленных [выше](#create-an-extension-in-a-new-resource-instance).</span><span class="sxs-lookup"><span data-stu-id="79b49-192">Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="79b49-193">Текст ответа</span><span class="sxs-lookup"><span data-stu-id="79b49-193">Response body</span></span>

| <span data-ttu-id="79b49-194">Сценарий</span><span class="sxs-lookup"><span data-stu-id="79b49-194">Scenario</span></span>       | <span data-ttu-id="79b49-195">Ресурс</span><span class="sxs-lookup"><span data-stu-id="79b49-195">Resource</span></span>  | <span data-ttu-id="79b49-196">Тело отклика</span><span class="sxs-lookup"><span data-stu-id="79b49-196">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="79b49-197">Создание расширения с явным созданием _нового_ экземпляра ресурса</span><span class="sxs-lookup"><span data-stu-id="79b49-197">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="79b49-198">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="79b49-198">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="79b49-199">Включает новый экземпляр, дополненный объектом [openTypeExtension](../resources/opentypeextension.md).</span><span class="sxs-lookup"><span data-stu-id="79b49-199">Includes the new instance expanded with the [openTypeExtension](../resources/opentypeextension.md) object.</span></span> |
| <span data-ttu-id="79b49-200">Создание расширения с неявным созданием экземпляра ресурса</span><span class="sxs-lookup"><span data-stu-id="79b49-200">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="79b49-201">post</span><span class="sxs-lookup"><span data-stu-id="79b49-201">post</span></span>](../resources/post.md) | <span data-ttu-id="79b49-202">Ответ содержит только код ответа без текста.</span><span class="sxs-lookup"><span data-stu-id="79b49-202">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="79b49-203">Создание расширения в _существующем_ экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="79b49-203">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="79b49-204">Все поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="79b49-204">All supported resources</span></span> | <span data-ttu-id="79b49-205">Включает объект **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="79b49-205">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="79b49-206">Пример</span><span class="sxs-lookup"><span data-stu-id="79b49-206">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="79b49-207">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="79b49-207">Request 1</span></span>

<span data-ttu-id="79b49-p109">В первом примере сообщение и расширение создаются в одном запросе. Текст запроса включает следующие данные:</span><span class="sxs-lookup"><span data-stu-id="79b49-p109">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="79b49-210">Свойства **subject**, **body** и **toRecipients**, характерные для нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="79b49-210">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="79b49-211">Данные для расширения:</span><span class="sxs-lookup"><span data-stu-id="79b49-211">And for the extension:</span></span>

  - <span data-ttu-id="79b49-212">Тип `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="79b49-212">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
  - <span data-ttu-id="79b49-213">Имя расширения "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="79b49-213">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="79b49-214">Дополнительные данные, хранимых в три настраиваемых свойств в полезных данных JSON: `companyName`, `expirationDate`, и `dealValue`.</span><span class="sxs-lookup"><span data-stu-id="79b49-214">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages

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
      "@odata.type": "Microsoft.Graph.OpenTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

### <a name="response-1"></a><span data-ttu-id="79b49-215">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="79b49-215">Response 1</span></span>

<span data-ttu-id="79b49-p110">Ниже представлен отклик для первого примера. Текст отклика включает свойства нового сообщения и следующие данные для нового расширения:</span><span class="sxs-lookup"><span data-stu-id="79b49-p110">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="79b49-218">Свойство **id** с полным именем `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="79b49-218">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="79b49-219">Стандартное свойство **extensionName**, указанное в запросе.</span><span class="sxs-lookup"><span data-stu-id="79b49-219">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="79b49-220">Пользовательские данные из запроса, сохраненные в виде 3 настраиваемых свойств.</span><span class="sxs-lookup"><span data-stu-id="79b49-220">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="79b49-p111">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79b49-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
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
  "extensions@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages
('AAMkAGEbs88AAB84uLuAAA%3D')/extensions",
  "extensions": [
    {
      "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
      "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
      "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

****

### <a name="request-2"></a><span data-ttu-id="79b49-223">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="79b49-223">Request 2</span></span>

<span data-ttu-id="79b49-p112">Во втором примере показано создание расширения в указанном сообщении. Текст запроса включает следующие данные для расширения:</span><span class="sxs-lookup"><span data-stu-id="79b49-p112">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="79b49-226">Тип `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="79b49-226">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="79b49-227">Имя расширения "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="79b49-227">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="79b49-228">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `dealValue` и `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="79b49-228">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```

### <a name="response-2"></a><span data-ttu-id="79b49-229">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="79b49-229">Response 2</span></span>

<span data-ttu-id="79b49-p113">Ниже представлен отклик для второго примера. Текст отклика включает следующие данные для нового расширения:</span><span class="sxs-lookup"><span data-stu-id="79b49-p113">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="79b49-232">Свойство по умолчанию **extensionName**.</span><span class="sxs-lookup"><span data-stu-id="79b49-232">The default property **extensionName**.</span></span>
- <span data-ttu-id="79b49-233">Свойство **id** с полным именем `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="79b49-233">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="79b49-234">Сохраняемые пользовательские данные.</span><span class="sxs-lookup"><span data-stu-id="79b49-234">The custom data to be stored.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

### <a name="request-3"></a><span data-ttu-id="79b49-235">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="79b49-235">Request 3</span></span>

<span data-ttu-id="79b49-p114">В третьем примере показано создание расширения в указанном событии группы. Текст запроса включает следующие данные для расширения:</span><span class="sxs-lookup"><span data-stu-id="79b49-p114">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="79b49-238">Тип `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="79b49-238">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="79b49-239">Имя расширения "Com.Contoso.Deal".</span><span class="sxs-lookup"><span data-stu-id="79b49-239">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="79b49-240">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `dealValue` и `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="79b49-240">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/beta/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

### <a name="response-3"></a><span data-ttu-id="79b49-241">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="79b49-241">Response 3</span></span>

<span data-ttu-id="79b49-242">Ниже представлен отклик из третьего примера.</span><span class="sxs-lookup"><span data-stu-id="79b49-242">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

### <a name="request-4"></a><span data-ttu-id="79b49-243">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="79b49-243">Request 4</span></span>

<span data-ttu-id="79b49-p115">В четвертом примере показано создание расширения в новой записи группы с помощью одного вызова действия **reply** для существующей записи группы. Действие **reply** создает запись и внедряет в нее новое расширение. Текст запроса включает свойство **post**, которое, в свою очередь, содержит свойство **body** новой записи и следующие данные для нового расширения:</span><span class="sxs-lookup"><span data-stu-id="79b49-p115">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="79b49-247">Тип `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="79b49-247">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="79b49-248">Имя расширения "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="79b49-248">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="79b49-249">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `expirationDate` и массив строк `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="79b49-249">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=')/reply

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
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

### <a name="response-4"></a><span data-ttu-id="79b49-250">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="79b49-250">Response 4</span></span>

<span data-ttu-id="79b49-p116">Ниже представлен отклик из четвертого примера. При успешном создании расширения в новой записи группы возвращается только код отклика HTTP 202.</span><span class="sxs-lookup"><span data-stu-id="79b49-p116">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

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

### <a name="request-5"></a><span data-ttu-id="79b49-253">Запрос 5</span><span class="sxs-lookup"><span data-stu-id="79b49-253">Request 5</span></span>

<span data-ttu-id="79b49-p117">В пятом примере показано создание расширения в новой записи группы с помощью той же операции POST, которая создает беседу. Операция POST создает беседу, цепочку и запись, а также внедряет в эту запись новое расширение. Текст отклика включает свойства **Topic** и **Threads**, а также дочерний объект **post** для новой беседы. Объект **post**, в свою очередь, содержит свойство **body** новой записи и следующие данные расширения:</span><span class="sxs-lookup"><span data-stu-id="79b49-p117">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="79b49-258">Тип `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="79b49-258">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="79b49-259">Имя расширения "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="79b49-259">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="79b49-260">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `expirationDate` и массив строк `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="79b49-260">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations

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
              "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
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

### <a name="response-5"></a><span data-ttu-id="79b49-261">Отклик 5</span><span class="sxs-lookup"><span data-stu-id="79b49-261">Response 5</span></span>

<span data-ttu-id="79b49-p118">Ниже представлен отклик из пятого примера, содержащий новую беседу и идентификатор цепочки. Эта новая цепочка содержит автоматически созданную запись, включающую новое расширение.</span><span class="sxs-lookup"><span data-stu-id="79b49-p118">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="79b49-p119">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79b49-p119">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="79b49-p120">Чтобы получить новое расширение, сначала [получите все записи](../api/conversationthread-list-posts.md) из цепочки. Изначально в ней должна быть только одна запись. Затем примените идентификатор записи и имя расширения `Com.Contoso.Benefits`, чтобы [получить расширение](../api/opentypeextension-get.md).</span><span class="sxs-lookup"><span data-stu-id="79b49-p120">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
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
