---
title: Создание команды
description: Создание новой команды.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: e34a095597064401f59ad5f78f8ca092e93b94b4
ms.sourcegitcommit: d91ca408bae7842ea4d1d94b49594fd82a32e0c9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2019
ms.locfileid: "29745533"
---
# <a name="create-team"></a><span data-ttu-id="d7479-103">Создание команды</span><span class="sxs-lookup"><span data-stu-id="d7479-103">Create team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7479-104">Создание новой [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d7479-104">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d7479-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7479-105">Permissions</span></span>

<span data-ttu-id="d7479-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7479-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7479-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7479-108">Permission type</span></span>                        | <span data-ttu-id="d7479-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7479-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d7479-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7479-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7479-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7479-111">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="d7479-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7479-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7479-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7479-113">Not supported.</span></span>                              |
| <span data-ttu-id="d7479-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7479-114">Application</span></span>                            | <span data-ttu-id="d7479-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7479-115">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d7479-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7479-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="d7479-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7479-117">Request headers</span></span>

| <span data-ttu-id="d7479-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7479-118">Header</span></span>        | <span data-ttu-id="d7479-119">Значение</span><span class="sxs-lookup"><span data-stu-id="d7479-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="d7479-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7479-120">Authorization</span></span> | <span data-ttu-id="d7479-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7479-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7479-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7479-123">Content-Type</span></span>  | <span data-ttu-id="d7479-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d7479-124">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="d7479-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7479-125">Request body</span></span>

<span data-ttu-id="d7479-126">Предоставьте в тексте запроса описание объекта [team](../resources/team.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7479-126">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d7479-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7479-127">Response</span></span>

<span data-ttu-id="d7479-128">В случае успешного выполнения этот API возвращает отклик `202 Accepted`, содержащий ссылку на [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="d7479-128">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="d7479-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="d7479-129">Examples</span></span>

### <a name="example-1-delegated-permissions"></a><span data-ttu-id="d7479-130">Пример 1. Делегированные разрешения</span><span class="sxs-lookup"><span data-stu-id="d7479-130">Example 1: Delegated permissions</span></span>

<span data-ttu-id="d7479-131">Ниже приведен пример минимального запроса.</span><span class="sxs-lookup"><span data-stu-id="d7479-131">The following is an example of a minimal request.</span></span> <span data-ttu-id="d7479-132">Исключив другие свойства, клиент неявно принимает значения по умолчанию из готового шаблона, представленного объектом `template`.</span><span class="sxs-lookup"><span data-stu-id="d7479-132">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="d7479-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7479-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description"
}
```

##### <a name="response"></a><span data-ttu-id="d7479-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7479-134">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-2-application-permissions"></a><span data-ttu-id="d7479-135">Пример 2. Разрешения для приложения</span><span class="sxs-lookup"><span data-stu-id="d7479-135">Example 2: Application permissions</span></span>

<span data-ttu-id="d7479-136">Ниже приведен пример минимального запроса с использованием разрешений для приложения.</span><span class="sxs-lookup"><span data-stu-id="d7479-136">The following is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="d7479-137">Исключив другие свойства, клиент неявно принимает значения по умолчанию из готового шаблона, представленного объектом `template`.</span><span class="sxs-lookup"><span data-stu-id="d7479-137">By omitting other properties, the client is implicitly taking defaults from the predefined template represented by `template`.</span></span> <span data-ttu-id="d7479-138">При отправке запроса с разрешениями для приложения ресурс [user](../resources/user.md) должен быть указан в коллекции `owners`.</span><span class="sxs-lookup"><span data-stu-id="d7479-138">When issuing a request with application permissions, a [user](../resources/user.md) must be specified in the `owners` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="d7479-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7479-139">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users('abc123')"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="d7479-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7479-140">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-3-create-a-team-with-an-app-installed-multiple-channels-with-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="d7479-141">Пример 3. Создание команды с установленным приложением и несколькими каналами с закрепленными вкладками с использованием делегированных разрешений</span><span class="sxs-lookup"><span data-stu-id="d7479-141">Example 3: Create a team with an app installed, multiple channels with pinned tabs using delegated permissions</span></span>

<span data-ttu-id="d7479-142">Ниже приведен запрос с указанием полного набора полезных данных.</span><span class="sxs-lookup"><span data-stu-id="d7479-142">The following is a request with a full payload.</span></span> <span data-ttu-id="d7479-143">Клиент может переопределить значения в базовом шаблоне и добавить элементы со значениями массива в пределах, допускаемых правилами проверки для объекта `specialization`.</span><span class="sxs-lookup"><span data-stu-id="d7479-143">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span> 

#### <a name="request"></a><span data-ttu-id="d7479-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7479-144">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
    "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
    "visibility": "Private",
    "displayName": "Sample Engineering Team",
    "description": "This is a sample engineering team, used to showcase the range of properties supported by this API",
    "channels": [
        {
            "displayName": "Announcements 📢",
            "isFavoriteByDefault": true,
            "description": "This is a sample announcements channel that is favorited by default. Use this channel to make important team, product, and service announcements."
        },
        {
            "displayName": "Training 🏋️",
            "isFavoriteByDefault": true,
            "description": "This is a sample training channel, that is favorited by default, and contains an example of pinned website and YouTube tabs.",
            "tabs": [
                {
                    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.web')",
                    "name": "A Pinned Website",
                    "configuration": {
                        "contentUrl": "https://docs.microsoft.com/en-us/microsoftteams/microsoft-teams"
                    }
                },
                {
                    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.youtube')",
                    "name": "A Pinned YouTube Video",
                    "configuration": {
                        "contentUrl": "https://tabs.teams.microsoft.com/Youtube/Home/YoutubeTab?videoId=X8krAMdGvCQ",
                        "websiteUrl": "https://www.youtube.com/watch?v=X8krAMdGvCQ"
                    }
                }
            ]
        },
        {
            "displayName": "Planning 📅 ",
            "description": "This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.",
            "isFavoriteByDefault": false
        },
        {
            "displayName": "Issues and Feedback 🐞",
            "description": "This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu."
        }
    ],
    "memberSettings": {
        "allowCreateUpdateChannels": true,
        "allowDeleteChannels": true,
        "allowAddRemoveApps": true,
        "allowCreateUpdateRemoveTabs": true,
        "allowCreateUpdateRemoveConnectors": true
    },
    "guestSettings": {
        "allowCreateUpdateChannels": false,
        "allowDeleteChannels": false
    },
    "funSettings": {
        "allowGiphy": true,
        "giphyContentRating": "Moderate",
        "allowStickersAndMemes": true,
        "allowCustomMemes": true
    },
    "messagingSettings": {
        "allowUserEditMessages": true,
        "allowUserDeleteMessages": true,
        "allowOwnerDeleteMessages": true,
        "allowTeamMentions": true,
        "allowChannelMentions": true
    },
    "installedApps": [
        {
            "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
        },
        {
            "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="d7479-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7479-145">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-4-create-a-team-with-a-non-standard-base-template-type"></a><span data-ttu-id="d7479-146">Пример 4. Создание команды с использованием нестандартного базового типа шаблона</span><span class="sxs-lookup"><span data-stu-id="d7479-146">Example 4: Create a team with a non-standard base template type</span></span>

<span data-ttu-id="d7479-147">Базовые типы шаблонов — это специальные шаблоны, созданные корпорацией Майкрософт для определенных отраслей.</span><span class="sxs-lookup"><span data-stu-id="d7479-147">Base template types are special templates that Microsoft created for specific industries.</span></span> <span data-ttu-id="d7479-148">Эти базовые шаблоны зачастую содержат защищаемые приложения, недоступные в свойствах хранилища и команды, которые еще не поддерживаются по отдельности в шаблонах Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d7479-148">These base templates often contain proprietary apps that aren't available in the store and team properties that are not yet supported individually in Microsoft Teams templates.</span></span>

<span data-ttu-id="d7479-149">Чтобы создать команду на основе нестандартного базового шаблона, потребуется изменить значение свойства `template@odata.bind` со `standard` на название этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="d7479-149">To create a team from a non-standard base template, you’ll want to change the `template@odata.bind` property in the request body from `standard` to point to the specific base template you’d like to create.</span></span>

<span data-ttu-id="d7479-150">Дополнительные сведения о поддерживаемых базовых типах шаблонов см. в статье [Начало работы с шаблонами Teams](https://docs.microsoft.com/ru-RU/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="d7479-150">To learn more about supported base template types, see [Get started with Teams templates](https://docs.microsoft.com/ru-RU/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="d7479-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7479-151">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/educationClass",
  "displayName": "My Class Team",
  "description": "My Class Team’s Description"
}
```

#### <a name="response"></a><span data-ttu-id="d7479-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7479-152">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-5-create-a-team-with-a-non-standard-base-template-type-with-extended-properties"></a><span data-ttu-id="d7479-153">Пример 5. Создание команды с использованием нестандартного базового типа шаблона с расширенными свойствами</span><span class="sxs-lookup"><span data-stu-id="d7479-153">Example 5: Create a team with a non-standard base template type with extended properties</span></span>

<span data-ttu-id="d7479-154">Базовые типы шаблонов могут быть расширены с помощью дополнительных свойств. Это позволяет дополнить существующий базовый шаблон дополнительными каналами, приложениями, вкладками и параметрами команды.</span><span class="sxs-lookup"><span data-stu-id="d7479-154">Base template types can be extended with additional properties, enabling you to build on an existing base template with additional team settings, channels, apps, or tabs.</span></span>

<span data-ttu-id="d7479-155">Дополнительные сведения о поддерживаемых базовых типах шаблонов и свойствах см. в статье [Начало работы с шаблонами Teams](https://docs.microsoft.com/ru-RU/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="d7479-155">To learn more about supported base template types and supported properties, see [Get started with Teams templates](https://docs.microsoft.com/ru-RU/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="d7479-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7479-156">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/educationClass",
  "displayName": "My Class Team",
  "description": "My Class Team’s Description",
  "channels": [
        {
            "displayName": "Class Announcements 📢",
            "isFavoriteByDefault": true
        },
        {
            "displayName": "Homework 🏋️",
            "isFavoriteByDefault": true,
        }
    ],
    "memberSettings": {
        "allowCreateUpdateChannels": false,
        "allowDeleteChannels": false,
        "allowAddRemoveApps": false,
        "allowCreateUpdateRemoveTabs": false,
        "allowCreateUpdateRemoveConnectors": false
    },
    "installedApps": [
        {
            "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
        },
        {
            "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="d7479-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7479-157">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

## <a name="see-also"></a><span data-ttu-id="d7479-158">См. также</span><span class="sxs-lookup"><span data-stu-id="d7479-158">See also</span></span>

- [<span data-ttu-id="d7479-159">Доступные шаблоны</span><span class="sxs-lookup"><span data-stu-id="d7479-159">Available templates</span></span>](https://docs.microsoft.com/ru-RU/MicrosoftTeams/get-started-with-teams-templates)
- [<span data-ttu-id="d7479-160">Начало работы с шаблонами команд розничной торговли</span><span class="sxs-lookup"><span data-stu-id="d7479-160">Getting started with Retail Teams templates</span></span>](https://docs.microsoft.com/MicrosoftTeams/get-started-with-retail-teams-templates)
- [<span data-ttu-id="d7479-161">Начало работы с шаблонами команд здравоохранения</span><span class="sxs-lookup"><span data-stu-id="d7479-161">Getting started with Healthcare Teams templates</span></span>](https://docs.microsoft.com/MicrosoftTeams/healthcare/healthcare-templates)
- [<span data-ttu-id="d7479-162">Создание группы с командой</span><span class="sxs-lookup"><span data-stu-id="d7479-162">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{/api-reference/beta/api/team-post.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
