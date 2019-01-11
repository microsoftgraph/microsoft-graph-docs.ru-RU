---
title: Создайте параметр каталога
description: Используйте этот интерфейс API для создания нового параметра, на основе шаблонов, доступных в directorySettingTemplates. Эти параметры можно на уровне клиента или на уровне объекта (в настоящее время только для групп). Запрос на создание необходимо задать settingValues для всех параметров, определенных в шаблоне. Для определенных параметров может устанавливаться только параметр Управление ли членов группы можно приглашать пользователей гостя. Преимущественную это поведение после общедоступной возможность добавления гостевых пользователей в группу.
localization_priority: Normal
ms.openlocfilehash: 692ca0d68522b5b268e9ee670c694e5a5c6bee90
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848722"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="41ee2-107">Создайте параметр каталога</span><span class="sxs-lookup"><span data-stu-id="41ee2-107">Create a directory setting</span></span>

> <span data-ttu-id="41ee2-108">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="41ee2-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41ee2-109">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41ee2-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41ee2-110">Используйте этот интерфейс API для создания нового параметра, на основе шаблонов, доступных в directorySettingTemplates.</span><span class="sxs-lookup"><span data-stu-id="41ee2-110">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="41ee2-111">Эти параметры можно на уровне клиента или на уровне объекта (в настоящее время только для групп).</span><span class="sxs-lookup"><span data-stu-id="41ee2-111">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="41ee2-112">Запрос на создание необходимо задать settingValues для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="41ee2-112">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="41ee2-113">Для определенных параметров может устанавливаться только параметр Управление ли членов группы можно приглашать пользователей гостя.</span><span class="sxs-lookup"><span data-stu-id="41ee2-113">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="41ee2-114">Преимущественную это поведение после общедоступной возможность добавления гостевых пользователей в группу.</span><span class="sxs-lookup"><span data-stu-id="41ee2-114">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="41ee2-115">**Примечание**: версия /beta этот интерфейс API является только относится к группам.</span><span class="sxs-lookup"><span data-stu-id="41ee2-115">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="41ee2-116">Версия /v1.0 этот интерфейс API переименовано в *Создание groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="41ee2-116">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="41ee2-117">Список шаблонов и свойств, которые они поддерживают в бета-версии используйте [directorySettingTemplate запроса](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span><span class="sxs-lookup"><span data-stu-id="41ee2-117">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="41ee2-118">(Для конечных точек версии 1.0, вызовите [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span><span class="sxs-lookup"><span data-stu-id="41ee2-118">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="41ee2-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41ee2-119">Permissions</span></span>
<span data-ttu-id="41ee2-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41ee2-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41ee2-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41ee2-122">Permission type</span></span>      | <span data-ttu-id="41ee2-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41ee2-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41ee2-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41ee2-124">Delegated (work or school account)</span></span> | <span data-ttu-id="41ee2-125">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="41ee2-125">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="41ee2-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41ee2-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41ee2-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41ee2-127">Not supported.</span></span>    |
|<span data-ttu-id="41ee2-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41ee2-128">Application</span></span> | <span data-ttu-id="41ee2-129">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41ee2-129">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41ee2-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41ee2-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="41ee2-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41ee2-131">Request headers</span></span>
| <span data-ttu-id="41ee2-132">Имя</span><span class="sxs-lookup"><span data-stu-id="41ee2-132">Name</span></span>       | <span data-ttu-id="41ee2-133">Описание</span><span class="sxs-lookup"><span data-stu-id="41ee2-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="41ee2-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41ee2-134">Authorization</span></span>  | <span data-ttu-id="41ee2-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41ee2-p107">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="41ee2-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="41ee2-137">Request body</span></span>
<span data-ttu-id="41ee2-138">В тексте запроса укажите представление JSON объекта [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="41ee2-138">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="41ee2-139">Тем не менее отображаемое имя для параметра задается в соответствии на имя шаблона параметров, который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="41ee2-139">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="41ee2-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="41ee2-140">Response</span></span>

<span data-ttu-id="41ee2-141">Успешно завершена, этот метод возвращает `201 Created` объект [directorySetting](../resources/directorysetting.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="41ee2-141">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41ee2-142">Пример</span><span class="sxs-lookup"><span data-stu-id="41ee2-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41ee2-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="41ee2-143">Request</span></span>
<span data-ttu-id="41ee2-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41ee2-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_settings"
}-->
```http
POST https://graph.microsoft.com/beta/settings
Content-type: application/json
Content-length: 222

{
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
<span data-ttu-id="41ee2-145">В тексте запроса укажите представление JSON объекта [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="41ee2-145">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="41ee2-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="41ee2-146">Response</span></span>
<span data-ttu-id="41ee2-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="41ee2-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
    "@odata.context": "https://graph.microsoft.com/stagingbeta/$metadata#settings/$entity",
    "id": "id-value",
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
