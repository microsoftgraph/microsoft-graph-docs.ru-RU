---
title: Как получить фотографию группы
description: Вы можете получить фотографию (изображение) для группы.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9531ef2c38033905bf14976345d7286bc4ab8a44
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290316"
---
# <a name="get-team-photo"></a><span data-ttu-id="2fbc0-103">Как получить фотографию группы</span><span class="sxs-lookup"><span data-stu-id="2fbc0-103">Get team photo</span></span>

<span data-ttu-id="2fbc0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fbc0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fbc0-105">Вы можете получить фотографию (изображение) для группы или метаданные этой фотографии.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-105">Get the photo (picture) for a team, or metadata for the photo.</span></span> <span data-ttu-id="2fbc0-106">В целом, лучше всего сначала попробовать извлечь метаданные о размере фотографии, которую вы хотите получить, чтобы убедиться в том, что этот размер доступен.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-106">In general, it is a best practice to first attempt to retrieve the metadata for the size of the photo you'd like to get to ensure that size is available.</span></span> <span data-ttu-id="2fbc0-107">После того как вы извлекли метаданные, используйте путь `/$value`, чтобы получить двоичные данные фотографии.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-107">Once you have retrieved the metadata, use the `/$value` path to get the binary data for the photo.</span></span>

<span data-ttu-id="2fbc0-108">Действуя этим методом, мы сначала пробуем извлечь указанную фотографию из Office 365.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-108">This method first attempts to retrieve the specified photo from Office 365.</span></span> <span data-ttu-id="2fbc0-109">Если фотография недоступна в Office 365, производится попытка извлечь ее из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-109">If the photo is not available in Office 365, it attempts to retrieve the photo from Azure Active Directory instead.</span></span>

<span data-ttu-id="2fbc0-110">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-110">The following are the supported sizes of HD photos in Office 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648 pixels.</span></span> <span data-ttu-id="2fbc0-111">Фотографии, хранящиеся в Azure Active Directory, могут быть любого размера.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-111">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="2fbc0-112">Вы можете получить метаданные самой большой доступной фотографии или указать размер и получить метаданные для фотографии этого размера.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-112">You can get the metadata of the largest available photo, or optionally specify a size to get the metadata for that photo size.</span></span> <span data-ttu-id="2fbc0-113">Если запрашиваемый размер недоступен, вы можете получить фотографию меньшего размера.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-113">If the size you request is not available, you can still get a smaller size.</span></span> <span data-ttu-id="2fbc0-114">Например, если самая крупная загруженная фотография имеет размер 504 x 504 пикселя, для скачивания будут доступны все размеры этой фотографии, кроме 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-114">For example, if the largest photo uploaded is 504x504 pixels, all but the 648x648 size of the photo will be available for download.</span></span> <span data-ttu-id="2fbc0-115">Если указанный размер недоступен в Office 365 или Azure Active Directory, возвращается размер 1 x 1 и остальные метаданные.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-115">If the specified size is not available in the Office 365 or in Azure Active Directory, the size 1x1 is returned with the rest of the metadata.</span></span>

> [!Note]
> <span data-ttu-id="2fbc0-116">Общий размер запроса REST не должен превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-116">There is a limit of 4 MB on the total size of the REST request.</span></span> <span data-ttu-id="2fbc0-117">Таким образом, размер фотографии составит менее 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-117">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fbc0-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2fbc0-118">Permissions</span></span>

<span data-ttu-id="2fbc0-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fbc0-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fbc0-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2fbc0-121">Permission type</span></span>      | <span data-ttu-id="2fbc0-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2fbc0-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fbc0-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2fbc0-123">Delegated (work or school account)</span></span> | <span data-ttu-id="2fbc0-124">Team. ReadBasic. ALL, Теамсеттингс. Read. ALL, Теамсеттингс. ReadWrite. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2fbc0-124">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="2fbc0-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2fbc0-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fbc0-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-126">Not supported.</span></span>    |
|<span data-ttu-id="2fbc0-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2fbc0-127">Application</span></span> | <span data-ttu-id="2fbc0-128">Теамсеттингс. Read. Group ([RSC](https://aka.ms/teams-rsc)), Теамсеттингс. Edit. Group ([RSC](https://aka.ms/teams-rsc)), Team. ReadBasic. ALL, Теамсеттингс. Read. ALL, Теамсеттингс. ReadWrite. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2fbc0-128">TeamSettings.Read.Group ([RSC](https://aka.ms/teams-rsc)), TeamSettings.Edit.Group ([RSC](https://aka.ms/teams-rsc)), Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fbc0-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2fbc0-129">HTTP request</span></span>

### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="2fbc0-130">Как получить метаданные фотографии</span><span class="sxs-lookup"><span data-stu-id="2fbc0-130">Get the metadata of the photo</span></span>

<span data-ttu-id="2fbc0-131">Эта конечная точка возвращает метаданные фотографии.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-131">This endpoint will return the metadata of the photo.</span></span> <span data-ttu-id="2fbc0-132">Если размер не указывать, возвращаются метаданные крупнейшей доступной фотографии.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-132">If no size is specified, the metadata for the largest photo size available will be returned.</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
GET /teams/{id}/photo
GET /teams/{id}/photo/{size}
```

### <a name="get-the-photo"></a><span data-ttu-id="2fbc0-133">Как получить фотографию</span><span class="sxs-lookup"><span data-stu-id="2fbc0-133">Get the photo</span></span>

<span data-ttu-id="2fbc0-134">Эта конечная точка извлекает двоичные данные для фотографии.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-134">This endpoint will retrieve the binary data for the photo.</span></span> <span data-ttu-id="2fbc0-135">Если размер не указан, возвращается наибольший доступный размер.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-135">If no size is specified, the largest size available will be returned.</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
GET /beta/teams/{id}/photo/$value
GET /beta/teams/{id}/photo/{size}/$value
```

## <a name="path-parameters"></a><span data-ttu-id="2fbc0-136">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="2fbc0-136">Path parameters</span></span>

<span data-ttu-id="2fbc0-137">Для этого метода поддерживается необязательный параметр пути, позволяющий указать размер фотографии, которую нужно извлечь.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-137">This method supports an optional path parameter to specify the size of the photo to be retrieved.</span></span> <span data-ttu-id="2fbc0-138">Можно указать любой размер вплоть до максимального доступного.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-138">You can specify any size up to the largest available size.</span></span> <span data-ttu-id="2fbc0-139">Чтобы определить максимальный доступный размер, получите метаданные фотографии.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-139">Get the photo metadata to determine the largest size available.</span></span>

|<span data-ttu-id="2fbc0-140">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="2fbc0-140">**Parameter**</span></span>|<span data-ttu-id="2fbc0-141">**Тип**</span><span class="sxs-lookup"><span data-stu-id="2fbc0-141">**Type**</span></span>|<span data-ttu-id="2fbc0-142">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2fbc0-142">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2fbc0-143">size</span><span class="sxs-lookup"><span data-stu-id="2fbc0-143">size</span></span>  |<span data-ttu-id="2fbc0-144">String</span><span class="sxs-lookup"><span data-stu-id="2fbc0-144">String</span></span>  | <span data-ttu-id="2fbc0-145">Размер фотографии.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-145">A photo size.</span></span> <span data-ttu-id="2fbc0-146">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-146">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="2fbc0-147">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-147">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> <span data-ttu-id="2fbc0-148">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-148">Optional.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2fbc0-149">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2fbc0-149">Request headers</span></span>

| <span data-ttu-id="2fbc0-150">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2fbc0-150">Header</span></span>        | <span data-ttu-id="2fbc0-151">Значение</span><span class="sxs-lookup"><span data-stu-id="2fbc0-151">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="2fbc0-152">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2fbc0-152">Authorization</span></span> | <span data-ttu-id="2fbc0-p111">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-p111">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2fbc0-155">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2fbc0-155">Request body</span></span>

<span data-ttu-id="2fbc0-156">Текст для этого запроса указывать не нужно.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-156">Do not supply a body for this request.</span></span>

## <a name="response"></a><span data-ttu-id="2fbc0-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fbc0-157">Response</span></span>

### <a name="response-for-getting-the-metadata-of-a-photo"></a><span data-ttu-id="2fbc0-158">Отклик при получении метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="2fbc0-158">Response for getting the metadata of a photo</span></span>

<span data-ttu-id="2fbc0-159">При успешной отправке запроса этим способом возвращаются код отклика`200 OK` и метаданные о запрашиваемой фотографии.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-159">If successful, this method returns a `200 OK` response code, and metadata about the photo.</span></span>

### <a name="response-for-getting-the-photo"></a><span data-ttu-id="2fbc0-160">Отклик при получении фотографии</span><span class="sxs-lookup"><span data-stu-id="2fbc0-160">Response for getting the photo</span></span>

<span data-ttu-id="2fbc0-161">При успешной отправке запроса этим способом возвращаются код отклика `200 OK` и двоичные данные запрашиваемой фотографии.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-161">If successful, this method returns a `200 OK` response code, and the binary data for the photo.</span></span>

## <a name="examples"></a><span data-ttu-id="2fbc0-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="2fbc0-162">Examples</span></span>

### <a name="example-1-get-the-photo-metadata"></a><span data-ttu-id="2fbc0-163">Пример 1. Как получить метаданные фотографии</span><span class="sxs-lookup"><span data-stu-id="2fbc0-163">Example 1: Get the photo metadata</span></span>

#### <a name="request"></a><span data-ttu-id="2fbc0-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fbc0-164">Request</span></span>

<span data-ttu-id="2fbc0-165">Ниже приведен пример запроса на получение метаданных фотографии группы.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-165">Here is an example of the request to get the metadata of the team photo.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo_metadata"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo
```

#### <a name="response"></a><span data-ttu-id="2fbc0-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fbc0-166">Response</span></span>

<span data-ttu-id="2fbc0-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-167">Here is an example of the response.</span></span>

> <span data-ttu-id="2fbc0-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ddfcd489-628b-7d04-b48b-20075df800e5')/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/teams('ddfcd489-628b-7d04-b48b-20075df800e5')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

### <a name="example-2-get-a-specific-size-of-the-team-photo"></a><span data-ttu-id="2fbc0-170">Пример 2. Как получить фотографию группы определенного размера</span><span class="sxs-lookup"><span data-stu-id="2fbc0-170">Example 2: Get a specific size of the team photo</span></span>

<span data-ttu-id="2fbc0-171">Вот пример запроса на получение фотографии группы определенного размера.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-171">Here is an example of the request to get the team photo in a specific size.</span></span>

#### <a name="request"></a><span data-ttu-id="2fbc0-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fbc0-172">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo/240x240/$value
```

#### <a name="response"></a><span data-ttu-id="2fbc0-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fbc0-173">Response</span></span>

<span data-ttu-id="2fbc0-174">Содержит двоичные данные запрошенной фотографии размера 240 х 240.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-174">Contains the binary data of the requested 240x240 photo.</span></span> <span data-ttu-id="2fbc0-175">Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="2fbc0-175">The HTTP response code is 200.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
