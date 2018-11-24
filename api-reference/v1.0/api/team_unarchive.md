# <a name="unarchive-team"></a><span data-ttu-id="41bcb-101">Unarchive группы</span><span class="sxs-lookup"><span data-stu-id="41bcb-101">Unarchive team</span></span>



<span data-ttu-id="41bcb-102">Восстановление архивированных [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="41bcb-102">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="41bcb-103">Это восстанавливает возможность отправлять сообщения и изменение группы, сотрудничает с параметры клиента и группы.</span><span class="sxs-lookup"><span data-stu-id="41bcb-103">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="41bcb-104">Команды, архивируются использования [архива](team_archive.md) API.</span><span class="sxs-lookup"><span data-stu-id="41bcb-104">Teams are archived using the [archive](team_archive.md) API.</span></span>

<span data-ttu-id="41bcb-105">Unarchiving является асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="41bcb-105">Unarchiving is an async operation.</span></span> <span data-ttu-id="41bcb-106">Группа архиве после асинхронного успешного завершения операции, которой может произойти после ответа от этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="41bcb-106">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="41bcb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41bcb-107">Permissions</span></span>
<span data-ttu-id="41bcb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="41bcb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="41bcb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41bcb-110">Permission type</span></span>      | <span data-ttu-id="41bcb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41bcb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41bcb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41bcb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="41bcb-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41bcb-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="41bcb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41bcb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41bcb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41bcb-115">Not supported.</span></span>    |
|<span data-ttu-id="41bcb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41bcb-116">Application</span></span> | <span data-ttu-id="41bcb-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41bcb-117">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="41bcb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41bcb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="41bcb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41bcb-119">Request headers</span></span>
| <span data-ttu-id="41bcb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41bcb-120">Header</span></span>       | <span data-ttu-id="41bcb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="41bcb-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="41bcb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41bcb-122">Authorization</span></span>  | <span data-ttu-id="41bcb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41bcb-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="41bcb-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41bcb-125">Request body</span></span>
<span data-ttu-id="41bcb-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41bcb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41bcb-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="41bcb-127">Response</span></span>

<span data-ttu-id="41bcb-128">Если unarchiving запускается успешно, этот метод возвращает `202 Accepted` код ответа.</span><span class="sxs-lookup"><span data-stu-id="41bcb-128">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="41bcb-129">Ответ также будет содержать `Location` заголовок, который содержит расположение [teamsAsyncOperation](../resources/teamsasyncoperation.md) , который был создан для обработки unarchiving рабочей группы.</span><span class="sxs-lookup"><span data-stu-id="41bcb-129">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="41bcb-130">Проверьте состояние unarchiving операции, внесение запрос GET в этом расположении.</span><span class="sxs-lookup"><span data-stu-id="41bcb-130">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="41bcb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="41bcb-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="41bcb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="41bcb-132">Request</span></span>
<span data-ttu-id="41bcb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41bcb-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="41bcb-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="41bcb-134">Response</span></span>
<span data-ttu-id="41bcb-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="41bcb-135">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
