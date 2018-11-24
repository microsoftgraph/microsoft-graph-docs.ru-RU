# <a name="archive-team"></a><span data-ttu-id="b955e-101">Группа архива</span><span class="sxs-lookup"><span data-stu-id="b955e-101">Archive team</span></span>



<span data-ttu-id="b955e-102">Архивируйте указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="b955e-102">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="b955e-103">При архивации группы, пользователи могут больше не отправлять или как сообщения на любом рабочих групп, изменить имя группы, описание или другие параметры или в целом изменять большинство в группу.</span><span class="sxs-lookup"><span data-stu-id="b955e-103">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="b955e-104">Изменения членства в группе продолжать разрешено.</span><span class="sxs-lookup"><span data-stu-id="b955e-104">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="b955e-105">Архивация — это асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="b955e-105">Archiving is an async operation.</span></span> <span data-ttu-id="b955e-106">Группа архивируется после асинхронного успешного завершения операции, которой может произойти после ответа от этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="b955e-106">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="b955e-107">Для архивации группы, группы и [группы](../resources/group.md) должен иметь владельца.</span><span class="sxs-lookup"><span data-stu-id="b955e-107">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="b955e-108">Чтобы восстановить группы из состояния архивных, используйте API-интерфейса [unarchive](team_unarchive.md).</span><span class="sxs-lookup"><span data-stu-id="b955e-108">To restore a team from its archived state, use the API to [unarchive](team_unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b955e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b955e-109">Permissions</span></span>
<span data-ttu-id="b955e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b955e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b955e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b955e-112">Permission type</span></span>      | <span data-ttu-id="b955e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b955e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b955e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b955e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b955e-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b955e-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b955e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b955e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b955e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b955e-117">Not supported.</span></span>    |
|<span data-ttu-id="b955e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b955e-118">Application</span></span> | <span data-ttu-id="b955e-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b955e-119">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="b955e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b955e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="b955e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b955e-121">Request headers</span></span>
| <span data-ttu-id="b955e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b955e-122">Header</span></span>       | <span data-ttu-id="b955e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b955e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b955e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b955e-124">Authorization</span></span>  | <span data-ttu-id="b955e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b955e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b955e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b955e-127">Request body</span></span>
<span data-ttu-id="b955e-128">В запросе, можно _Дополнительно_ включить `shouldSetSpoSiteReadOnlyForMembers` параметр в формате JSON в body следующим образом.</span><span class="sxs-lookup"><span data-stu-id="b955e-128">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="b955e-129">Этот дополнительный параметр определяет, требуется ли задавать разрешения для членов группы только для чтения на сайте Sharepoint Online, связанный с группой.</span><span class="sxs-lookup"><span data-stu-id="b955e-129">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="b955e-130">Задать значение false или пропуск текста полностью приведет к этот шаг пропущен.</span><span class="sxs-lookup"><span data-stu-id="b955e-130">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="b955e-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="b955e-131">Response</span></span>

<span data-ttu-id="b955e-132">Если архивация запускается успешно, этот метод возвращает `202 Accepted` код ответа.</span><span class="sxs-lookup"><span data-stu-id="b955e-132">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="b955e-133">Ответ также будет содержать `Location` заголовок, который содержит расположение [teamsAsyncOperation](../resources/teamsasyncoperation.md) , который был создан для обработки архивации рабочей группы.</span><span class="sxs-lookup"><span data-stu-id="b955e-133">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="b955e-134">Проверьте состояние архивации операции, внесение запрос GET в этом расположении.</span><span class="sxs-lookup"><span data-stu-id="b955e-134">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="b955e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="b955e-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b955e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="b955e-136">Request</span></span>
<span data-ttu-id="b955e-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b955e-137">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="b955e-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="b955e-138">Response</span></span>
<span data-ttu-id="b955e-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b955e-139">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
