# <a name="force-domain-deletion"></a><span data-ttu-id="ca031-101">Принудительно удалить домен</span><span class="sxs-lookup"><span data-stu-id="ca031-101">Force domain deletion</span></span>

<span data-ttu-id="ca031-102">Удаление домена, с помощью асинхронной операции длительным.</span><span class="sxs-lookup"><span data-stu-id="ca031-102">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="ca031-103">В рамках этой операции выполняются следующие действия:</span><span class="sxs-lookup"><span data-stu-id="ca031-103">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="ca031-104">Обновления `userPrincipalName`, `mail`, и `proxyAddresses` свойства `users` со ссылками на удаленный домен, используемый домена начальной onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="ca031-104">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="ca031-105">Обновления `mail` свойства `groups` со ссылками на удаленный домен, используемый домена начальной onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="ca031-105">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="ca031-106">Обновления `identifierUris` свойства `applications` со ссылками на удаленный домен, используемый домена начальной onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="ca031-106">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="ca031-107">Если число объектов, чтобы переименовать больше 1000, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="ca031-107">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="ca031-108">При выполнении одного из `applications` Чтобы переименовать приложения нескольких развертываний, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="ca031-108">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="ca031-109">После завершения удаления домена операции API для удаленного домена возвращает код состояния HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="ca031-109">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="ca031-110">Чтобы подтвердить удаление домена, можно выполнить операции [get домена](domain_get.md) .</span><span class="sxs-lookup"><span data-stu-id="ca031-110">To verify deletion of a domain, you can perform a [get domain](domain_get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca031-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca031-111">Permissions</span></span>

<span data-ttu-id="ca031-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ca031-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ca031-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca031-114">Permission type</span></span>      | <span data-ttu-id="ca031-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca031-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca031-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca031-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ca031-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ca031-117">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ca031-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca031-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca031-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca031-119">Not supported.</span></span>    |
|<span data-ttu-id="ca031-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca031-120">Application</span></span> | <span data-ttu-id="ca031-121">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca031-121">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca031-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca031-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="ca031-123">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="ca031-123">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca031-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca031-124">Request headers</span></span>

| <span data-ttu-id="ca031-125">Имя</span><span class="sxs-lookup"><span data-stu-id="ca031-125">Name</span></span> | <span data-ttu-id="ca031-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ca031-126">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ca031-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca031-127">Authorization</span></span>  | <span data-ttu-id="ca031-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca031-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="ca031-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca031-130">Content-Type</span></span>  | <span data-ttu-id="ca031-131">application/json</span><span class="sxs-lookup"><span data-stu-id="ca031-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca031-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca031-132">Request body</span></span>

<span data-ttu-id="ca031-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ca031-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ca031-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="ca031-134">Parameter</span></span> | <span data-ttu-id="ca031-135">Тип</span><span class="sxs-lookup"><span data-stu-id="ca031-135">Type</span></span> | <span data-ttu-id="ca031-136">Описание</span><span class="sxs-lookup"><span data-stu-id="ca031-136">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="ca031-137">Параметр, чтобы отключить учетные записи пользователей, которые были изменены при переносе.</span><span class="sxs-lookup"><span data-stu-id="ca031-137">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="ca031-138">Если учетная запись пользователя отключена, пользователь не разрешено вход.</span><span class="sxs-lookup"><span data-stu-id="ca031-138">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="ca031-139">Если задано значение **true** `users` обновлена как часть этой операции будут отключены.</span><span class="sxs-lookup"><span data-stu-id="ca031-139">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="ca031-140">Значение по умолчанию — **true**.</span><span class="sxs-lookup"><span data-stu-id="ca031-140">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="ca031-141">Текст ответа</span><span class="sxs-lookup"><span data-stu-id="ca031-141">Response body</span></span>

<span data-ttu-id="ca031-142">Успешно завершена, этот метод возвращает `HTTP/1.1 204 OK` код состояния.</span><span class="sxs-lookup"><span data-stu-id="ca031-142">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="ca031-143">Пример</span><span class="sxs-lookup"><span data-stu-id="ca031-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca031-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca031-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/beta/domains/{id}/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```

### <a name="response"></a><span data-ttu-id="ca031-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca031-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->