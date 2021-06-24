---
title: 'присутствие: setPresence'
description: Установите сведения о присутствии для сеанса присутствия приложения пользователя.
author: jsandoval-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: d403cf8e828ecebb1e08164657ac1adb8191f57f
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107865"
---
# <a name="presence-setpresence"></a><span data-ttu-id="24437-103">присутствие: setPresence</span><span class="sxs-lookup"><span data-stu-id="24437-103">presence: setPresence</span></span>

<span data-ttu-id="24437-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24437-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24437-105">Установите состояние сеанса присутствия пользователя в качестве приложения.</span><span class="sxs-lookup"><span data-stu-id="24437-105">Set the state of a user's presence session as an application.</span></span>

### <a name="presence-sessions"></a><span data-ttu-id="24437-106">Сеансы присутствия</span><span class="sxs-lookup"><span data-stu-id="24437-106">Presence sessions</span></span>
<span data-ttu-id="24437-107">У пользователя может быть несколько сеансов присутствия, так как он может быть на нескольких Teams (настольных, мобильных и веб-).</span><span class="sxs-lookup"><span data-stu-id="24437-107">A user can have multiple presence sessions because the user can be on multiple Teams clients (desktop, mobile, and web).</span></span> <span data-ttu-id="24437-108">Каждый Teams клиент имеет сеанс независимого присутствия, а присутствие пользователя — это агрегированное состояние из всех сеансов позади.</span><span class="sxs-lookup"><span data-stu-id="24437-108">Each Teams client has an independent presence session and the user's presence is an aggregated state from all the sessions behind.</span></span>

<span data-ttu-id="24437-109">Кроме того, приложение может иметь свое собственное сеанс присутствия для пользователя и иметь возможность обновлять состояние.</span><span class="sxs-lookup"><span data-stu-id="24437-109">Similarly, an application can have its own presence session for a user and be able to update the state.</span></span>

<span data-ttu-id="24437-110">Ниже приводится преимущество агрегированного состояния сеанса:</span><span class="sxs-lookup"><span data-stu-id="24437-110">The following is the precedence for how session states are aggregated:</span></span>
* <span data-ttu-id="24437-111">Настраиваемое пользователем > настраиваемое приложением (состояние, настроенное пользователем, переопределяет другие)</span><span class="sxs-lookup"><span data-stu-id="24437-111">User-configured > app-configured (user-configured state overrides others)</span></span>
* <span data-ttu-id="24437-112">Среди настраиваемых приложений: DoNotDisturb (в настоящее время не поддерживается для набора присутствия) > Busy > Доступно > Away</span><span class="sxs-lookup"><span data-stu-id="24437-112">Among app-configured: DoNotDisturb (currently not supported for set presence) > Busy > Available > Away</span></span>

### <a name="timeout-expiration-and-keep-alive"></a><span data-ttu-id="24437-113">Время ожидания, срок действия и сохранение</span><span class="sxs-lookup"><span data-stu-id="24437-113">Timeout, expiration, and keep alive</span></span>
<span data-ttu-id="24437-114">Сеанс присутствия может **быть** выходным и истекает, поэтому приложению необходимо вызвать этот API перед выходом **времени,** чтобы сохранить состояние сеанса; или до истечения **срока действия,** чтобы сохранить сеанс в живых.</span><span class="sxs-lookup"><span data-stu-id="24437-114">A presence session may **time out** and **expire**, so the application needs to call this API before the **timeout**, to maintain the state for the session; or before the **expiration**, to keep the session alive.</span></span>

<span data-ttu-id="24437-115">Сеанс присутствия может быть отсуттсвуем, если доступность и `Available` время в 5 минут.</span><span class="sxs-lookup"><span data-stu-id="24437-115">A presence session can time out if the availability is `Available` and the timeout is 5 minutes.</span></span> <span data-ttu-id="24437-116">При разовом периоде состояние присутствия постепенно исчезает.</span><span class="sxs-lookup"><span data-stu-id="24437-116">When it times out, the presence state fades in stages.</span></span> <span data-ttu-id="24437-117">Например, если приложение задает сеанс присутствия в качестве, состояние изменится на 5 минут с первым таймаутом, а затем через 5 минут со вторым `Available/Available` `Available/AvailableInactive` `Away/Away` таймаутом.</span><span class="sxs-lookup"><span data-stu-id="24437-117">For example, if an application sets the presence session as `Available/Available`, the state would change to `Available/AvailableInactive` in 5 minutes with the first timeout, then `Away/Away` in another 5 minutes with the second timeout.</span></span>

<span data-ttu-id="24437-118">Срок действия сеанса присутствия настраивается с помощью `expirationDuration` параметра.</span><span class="sxs-lookup"><span data-stu-id="24437-118">The expiration of a presence session is configurable with the `expirationDuration` parameter.</span></span> <span data-ttu-id="24437-119">По истечении срока действия сеанса он становится `Offline` .</span><span class="sxs-lookup"><span data-stu-id="24437-119">When a session expires it becomes `Offline`.</span></span>

## <a name="permissions"></a><span data-ttu-id="24437-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24437-120">Permissions</span></span>
<span data-ttu-id="24437-121">Для вызова API требуется следующее разрешение.</span><span class="sxs-lookup"><span data-stu-id="24437-121">The following permission is required to call the API.</span></span> <span data-ttu-id="24437-122">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24437-122">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24437-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24437-123">Permission type</span></span>                        | <span data-ttu-id="24437-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24437-124">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="24437-125">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24437-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="24437-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24437-126">Not Supported.</span></span>                              |
| <span data-ttu-id="24437-127">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24437-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24437-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24437-128">Not Supported.</span></span>                              |
| <span data-ttu-id="24437-129">Приложение</span><span class="sxs-lookup"><span data-stu-id="24437-129">Application</span></span>                            | <span data-ttu-id="24437-130">Presence.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24437-130">Presence.ReadWrite.All</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="24437-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24437-131">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/setPresence
```
## <a name="request-headers"></a><span data-ttu-id="24437-132">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="24437-132">Request headers</span></span>
| <span data-ttu-id="24437-133">Имя</span><span class="sxs-lookup"><span data-stu-id="24437-133">Name</span></span>          | <span data-ttu-id="24437-134">Описание</span><span class="sxs-lookup"><span data-stu-id="24437-134">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="24437-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24437-135">Authorization</span></span> | <span data-ttu-id="24437-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24437-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="24437-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="24437-138">Content-Type</span></span>  | <span data-ttu-id="24437-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24437-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24437-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24437-141">Request body</span></span>

<span data-ttu-id="24437-142">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="24437-142">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="24437-143">Параметр</span><span class="sxs-lookup"><span data-stu-id="24437-143">Parameter</span></span>          | <span data-ttu-id="24437-144">Тип</span><span class="sxs-lookup"><span data-stu-id="24437-144">Type</span></span>     | <span data-ttu-id="24437-145">Описание</span><span class="sxs-lookup"><span data-stu-id="24437-145">Description</span></span>                                                                                            |
| :----------------- | :------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="24437-146">sessionId</span><span class="sxs-lookup"><span data-stu-id="24437-146">sessionId</span></span>          | <span data-ttu-id="24437-147">string</span><span class="sxs-lookup"><span data-stu-id="24437-147">string</span></span>   | <span data-ttu-id="24437-148">ID сеанса присутствия приложения.</span><span class="sxs-lookup"><span data-stu-id="24437-148">The ID of the application's presence session.</span></span>                                                          |
| <span data-ttu-id="24437-149">availability</span><span class="sxs-lookup"><span data-stu-id="24437-149">availability</span></span>       | <span data-ttu-id="24437-150">string</span><span class="sxs-lookup"><span data-stu-id="24437-150">string</span></span>   | <span data-ttu-id="24437-151">Сведения о базовом присутствии.</span><span class="sxs-lookup"><span data-stu-id="24437-151">The base presence information.</span></span>                                                                         |
| <span data-ttu-id="24437-152">действие</span><span class="sxs-lookup"><span data-stu-id="24437-152">activity</span></span>           | <span data-ttu-id="24437-153">string</span><span class="sxs-lookup"><span data-stu-id="24437-153">string</span></span>   | <span data-ttu-id="24437-154">Дополнительные сведения о доступности.</span><span class="sxs-lookup"><span data-stu-id="24437-154">The supplemental information to availability.</span></span>                                                          |
| <span data-ttu-id="24437-155">expirationDuration</span><span class="sxs-lookup"><span data-stu-id="24437-155">expirationDuration</span></span> | <span data-ttu-id="24437-156">duration</span><span class="sxs-lookup"><span data-stu-id="24437-156">duration</span></span> | <span data-ttu-id="24437-157">Срок действия сеанса присутствия приложения.</span><span class="sxs-lookup"><span data-stu-id="24437-157">The expiration of the app presence session.</span></span> <span data-ttu-id="24437-158">Значение представлено в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="24437-158">The value is represented in ISO 8601 format for durations.</span></span> |

> [!IMPORTANT]
>
> <span data-ttu-id="24437-159">Предоставление ID приложения, как `sessionId` и в запросе.</span><span class="sxs-lookup"><span data-stu-id="24437-159">Provide the ID of the application as `sessionId` in the request.</span></span>

<span data-ttu-id="24437-160">Поддерживаемые сочетания `availability` и `activity` являются:</span><span class="sxs-lookup"><span data-stu-id="24437-160">Supported combinations of `availability` and `activity` are:</span></span>

| <span data-ttu-id="24437-161">availability</span><span class="sxs-lookup"><span data-stu-id="24437-161">availability</span></span> | <span data-ttu-id="24437-162">действие</span><span class="sxs-lookup"><span data-stu-id="24437-162">activity</span></span>          | <span data-ttu-id="24437-163">Описание</span><span class="sxs-lookup"><span data-stu-id="24437-163">Description</span></span>                                              |
| :----------- | :---------------- | :------------------------------------------------------- |
| <span data-ttu-id="24437-164">Available</span><span class="sxs-lookup"><span data-stu-id="24437-164">Available</span></span>    | <span data-ttu-id="24437-165">Available</span><span class="sxs-lookup"><span data-stu-id="24437-165">Available</span></span>         | <span data-ttu-id="24437-166">Обновляет сеанс присутствия как доступный.</span><span class="sxs-lookup"><span data-stu-id="24437-166">Updates the presence session as Available.</span></span>               |
| <span data-ttu-id="24437-167">Занята</span><span class="sxs-lookup"><span data-stu-id="24437-167">Busy</span></span>         | <span data-ttu-id="24437-168">InACall</span><span class="sxs-lookup"><span data-stu-id="24437-168">InACall</span></span>           | <span data-ttu-id="24437-169">Обновляет сеанс присутствия как Busy, InACall.</span><span class="sxs-lookup"><span data-stu-id="24437-169">Updates the presence session as Busy, InACall.</span></span>           |
| <span data-ttu-id="24437-170">Занята</span><span class="sxs-lookup"><span data-stu-id="24437-170">Busy</span></span>         | <span data-ttu-id="24437-171">InAConferenceCall</span><span class="sxs-lookup"><span data-stu-id="24437-171">InAConferenceCall</span></span> | <span data-ttu-id="24437-172">Обновляет сеанс присутствия как Busy, InAConferenceCall.</span><span class="sxs-lookup"><span data-stu-id="24437-172">Updates the presence session as Busy, InAConferenceCall.</span></span> |
| <span data-ttu-id="24437-173">Away</span><span class="sxs-lookup"><span data-stu-id="24437-173">Away</span></span>         | <span data-ttu-id="24437-174">Away</span><span class="sxs-lookup"><span data-stu-id="24437-174">Away</span></span>              | <span data-ttu-id="24437-175">Обновляет сеанс присутствия как Away.</span><span class="sxs-lookup"><span data-stu-id="24437-175">Updates the presence session as Away.</span></span>                    |

## <a name="response"></a><span data-ttu-id="24437-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="24437-176">Response</span></span>
<span data-ttu-id="24437-177">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="24437-177">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="24437-178">Примеры</span><span class="sxs-lookup"><span data-stu-id="24437-178">Examples</span></span>
<span data-ttu-id="24437-179">В следующем запросе показано приложение с ИД, которое `22553876-f5ab-4529-bffb-cfe50aa89f87` задает сеанс присутствия для `fa8bf3dc-eca7-46b7-bad1-db199b62afc3` пользователя.</span><span class="sxs-lookup"><span data-stu-id="24437-179">The following request shows the application with ID `22553876-f5ab-4529-bffb-cfe50aa89f87` that sets its presence session for user `fa8bf3dc-eca7-46b7-bad1-db199b62afc3`.</span></span>

### <a name="request"></a><span data-ttu-id="24437-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="24437-180">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "set-presence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/setPresence
Content-Type: application/json

{
  "sessionId": "22553876-f5ab-4529-bffb-cfe50aa89f87",
  "availability": "Available",
  "activity": "Available",
  "expirationDuration": "PT1H"
}
```

### <a name="response"></a><span data-ttu-id="24437-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="24437-181">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
