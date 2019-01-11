---
title: Клонирование группы
description: Создайте копию группы. Эта операция также создает копию соответствующей группе.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 262cbe4bd17cc1ab3abded49b65868d0b8039e70
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854595"
---
# <a name="clone-a-team"></a><span data-ttu-id="018e1-104">Клонирование группы</span><span class="sxs-lookup"><span data-stu-id="018e1-104">Clone a team</span></span>

> <span data-ttu-id="018e1-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="018e1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="018e1-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="018e1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="018e1-107">Создайте копию [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="018e1-107">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="018e1-108">Эта операция также создает копию в соответствующие [группы](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="018e1-108">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="018e1-109">Можно определить какие части группы следует скопировать.</span><span class="sxs-lookup"><span data-stu-id="018e1-109">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="018e1-110">**приложения** - группами Майкрософт копий приложений, установленных в группе.</span><span class="sxs-lookup"><span data-stu-id="018e1-110">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="018e1-111">**каналы** — копирует структуру канала (но не сообщения в канале).</span><span class="sxs-lookup"><span data-stu-id="018e1-111">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="018e1-112">**члены** — копирует участников и владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="018e1-112">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="018e1-113">**Параметры** — копирует все параметры в рамках рабочей группы, а также параметры ключа группы.</span><span class="sxs-lookup"><span data-stu-id="018e1-113">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="018e1-114">**вкладки** — копирует вкладок между каналами.</span><span class="sxs-lookup"><span data-stu-id="018e1-114">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="018e1-115">При клонировании вкладок они помещаются в исходное состояние — они отображаются в панели вкладок в группах Microsoft и при первом открытии, вы перейдете через экрана конфигурации.</span><span class="sxs-lookup"><span data-stu-id="018e1-115">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="018e1-116">(Если пользователь на вкладке не имеет разрешения для настройки приложения, они появится сообщение о том, что вкладке еще не были настроены.)</span><span class="sxs-lookup"><span data-stu-id="018e1-116">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="018e1-117">Клонирование — это длительная операция.</span><span class="sxs-lookup"><span data-stu-id="018e1-117">Cloning is a long-running operation.</span></span>
<span data-ttu-id="018e1-118">После возвращает клонированной POST, необходимо получить [операция](../resources/teamsasyncoperation.md) , является ли он «запуск» или «успешно» и «failed».</span><span class="sxs-lookup"><span data-stu-id="018e1-118">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="018e1-119">Следует продолжить GET, пока состояние не «выполняется».</span><span class="sxs-lookup"><span data-stu-id="018e1-119">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="018e1-120">Рекомендуемые задержки между получает — 5 секунд.</span><span class="sxs-lookup"><span data-stu-id="018e1-120">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="018e1-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="018e1-121">Permissions</span></span>

<span data-ttu-id="018e1-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="018e1-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="018e1-124">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="018e1-124">Permission type</span></span>      | <span data-ttu-id="018e1-125">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="018e1-125">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="018e1-126">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="018e1-126">Delegated (work or school account)</span></span>     | <span data-ttu-id="018e1-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="018e1-127">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="018e1-128">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="018e1-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="018e1-129">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="018e1-129">Not supported.</span></span>    |
|<span data-ttu-id="018e1-130">Для приложений</span><span class="sxs-lookup"><span data-stu-id="018e1-130">Application</span></span>                            | <span data-ttu-id="018e1-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="018e1-131">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="018e1-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="018e1-132">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="018e1-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="018e1-133">Request headers</span></span>
| <span data-ttu-id="018e1-134">Заголовок</span><span class="sxs-lookup"><span data-stu-id="018e1-134">Header</span></span>       | <span data-ttu-id="018e1-135">Значение</span><span class="sxs-lookup"><span data-stu-id="018e1-135">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="018e1-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="018e1-136">Authorization</span></span>  | <span data-ttu-id="018e1-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="018e1-p107">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="018e1-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="018e1-139">Content-Type</span></span>  | <span data-ttu-id="018e1-140">application/json</span><span class="sxs-lookup"><span data-stu-id="018e1-140">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="018e1-141">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="018e1-141">Request body</span></span>

| <span data-ttu-id="018e1-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="018e1-142">Property</span></span>     | <span data-ttu-id="018e1-143">Тип</span><span class="sxs-lookup"><span data-stu-id="018e1-143">Type</span></span>   |<span data-ttu-id="018e1-144">Описание</span><span class="sxs-lookup"><span data-stu-id="018e1-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="018e1-145">classification</span><span class="sxs-lookup"><span data-stu-id="018e1-145">classification</span></span>|<span data-ttu-id="018e1-146">String (необязательно)</span><span class="sxs-lookup"><span data-stu-id="018e1-146">String (optional)</span></span>|<span data-ttu-id="018e1-147">Описание классификации для группы (например, низкий, средний или высокий для бизнеса).</span><span class="sxs-lookup"><span data-stu-id="018e1-147">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="018e1-148">Допустимые значения для этого свойства определены, создав значение [параметра](../resources/directorysetting.md) ClassificationList на основе [определения шаблона](../resources/directorysettingtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="018e1-148">Valid values for this property are defined by creating a ClassificationList [setting](../resources/directorysetting.md) value, based on the [template definition](../resources/directorysettingtemplate.md).</span></span> <span data-ttu-id="018e1-149">Если классификация не указан, классификации копируются из исходной группы или группы.</span><span class="sxs-lookup"><span data-stu-id="018e1-149">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="018e1-150">description</span><span class="sxs-lookup"><span data-stu-id="018e1-150">description</span></span>|<span data-ttu-id="018e1-151">String (необязательно)</span><span class="sxs-lookup"><span data-stu-id="018e1-151">String (optional)</span></span>|<span data-ttu-id="018e1-152">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="018e1-152">An optional description for the group.</span></span> <span data-ttu-id="018e1-153">Если это свойство не указан, он остается пустым.</span><span class="sxs-lookup"><span data-stu-id="018e1-153">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="018e1-154">displayName</span><span class="sxs-lookup"><span data-stu-id="018e1-154">displayName</span></span>|<span data-ttu-id="018e1-155">String</span><span class="sxs-lookup"><span data-stu-id="018e1-155">String</span></span>|<span data-ttu-id="018e1-p110">Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="018e1-p110">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="018e1-159">mailNickname</span><span class="sxs-lookup"><span data-stu-id="018e1-159">mailNickname</span></span>|<span data-ttu-id="018e1-160">String</span><span class="sxs-lookup"><span data-stu-id="018e1-160">String</span></span>|<span data-ttu-id="018e1-161">Псевдоним почты для группы, уникальные в организации.</span><span class="sxs-lookup"><span data-stu-id="018e1-161">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="018e1-162">Это свойство должен быть указан при создании группы.</span><span class="sxs-lookup"><span data-stu-id="018e1-162">This property must be specified when a group is created.</span></span> <span data-ttu-id="018e1-163">Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="018e1-163">Supports $filter.</span></span> <span data-ttu-id="018e1-164">Если это свойство не задано, его повторное вычисление из displayName.</span><span class="sxs-lookup"><span data-stu-id="018e1-164">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="018e1-165">Известные проблемы: это свойство учитывается.</span><span class="sxs-lookup"><span data-stu-id="018e1-165">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="018e1-166">partsToClone</span><span class="sxs-lookup"><span data-stu-id="018e1-166">partsToClone</span></span>| [<span data-ttu-id="018e1-167">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="018e1-167">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="018e1-168">Список разделенных запятой частей следует скопировать.</span><span class="sxs-lookup"><span data-stu-id="018e1-168">A comma-seperated list of the parts to clone.</span></span> <span data-ttu-id="018e1-169">Юридические части, «приложений, вкладок, параметры, каналы, участники».</span><span class="sxs-lookup"><span data-stu-id="018e1-169">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="018e1-170">visibility</span><span class="sxs-lookup"><span data-stu-id="018e1-170">visibility</span></span>|<span data-ttu-id="018e1-171">[teamVisibilityType](../resources/teamvisibilitytype.md) (необязательно)</span><span class="sxs-lookup"><span data-stu-id="018e1-171">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="018e1-172">Определяет видимость группы.</span><span class="sxs-lookup"><span data-stu-id="018e1-172">Specifies the visibility of the group.</span></span> <span data-ttu-id="018e1-173">Возможные значения: **частный**, **открытым**.</span><span class="sxs-lookup"><span data-stu-id="018e1-173">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="018e1-174">Если видимости не указан, видимости копируются из исходной группы или группы.</span><span class="sxs-lookup"><span data-stu-id="018e1-174">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="018e1-175">Если группа клонировании — это группа **educationClass** , параметр видимости игнорируется и видимости новой группы будут иметь значение HiddenMembership.</span><span class="sxs-lookup"><span data-stu-id="018e1-175">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="018e1-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="018e1-176">Response</span></span>

<span data-ttu-id="018e1-177">Если успешно завершена, этот метод возвращает `202 Accepted` код ответа с расположением: заголовок, с указанием ресурсов [операции](../resources/teamsasyncoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="018e1-177">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="018e1-178">После завершения операции ресурсов операции сообщит вам, идентификатор созданного группы.</span><span class="sxs-lookup"><span data-stu-id="018e1-178">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="018e1-179">Пример</span><span class="sxs-lookup"><span data-stu-id="018e1-179">Example</span></span>
#### <a name="request"></a><span data-ttu-id="018e1-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="018e1-180">Request</span></span>
<span data-ttu-id="018e1-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="018e1-181">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
POST /teams/{id}/clone
Content-Type: application/json

{  
     "displayName": "Library Assist",
     "description": "Self help community for library",
     "mailNickname": "libassist",
     "partsToClone": "apps,tabs,settings,channels,members",
     "visibility": "public"
}
```

#### <a name="response"></a><span data-ttu-id="018e1-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="018e1-182">Response</span></span>
<span data-ttu-id="018e1-183">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="018e1-183">The following is an example of the response.</span></span> <span data-ttu-id="018e1-184">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="018e1-184">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="018e1-185">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="018e1-185">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
