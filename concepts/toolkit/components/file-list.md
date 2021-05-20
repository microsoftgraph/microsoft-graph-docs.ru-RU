---
title: Компонент списка файлов в microsoft Graph набор средств
description: Компонент списка файлов используется для отображения списка файлов, показывая их значок и имя
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: 77eb93bc17d9c684ac61fc6a7dc2f263e406bba8
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579855"
---
# <a name="file-list-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="15372-103">Компонент списка файлов в microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="15372-103">File list component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="15372-104">Компонент Списка файлов [](/graph/api/resources/onedrive) отображает список нескольких папок и файлов с помощью имени файла или папки, значка и других свойств, которые вы указываете.</span><span class="sxs-lookup"><span data-stu-id="15372-104">The File List component displays [a list of multiple folders and files](/graph/api/resources/onedrive) by using the file/folder name, an icon, and other properties that you specify.</span></span> <span data-ttu-id="15372-105">Этот компонент использует [компонент mgt-file.](./file.md)</span><span class="sxs-lookup"><span data-stu-id="15372-105">This component uses the [mgt-file](./file.md) component.</span></span> <span data-ttu-id="15372-106">Вы можете указать определенный диск или сайт, отобразить список файлов, основанный на типе insight (трендовые, используемые или общие), или предоставить запросы в настраиваемый список файлов.</span><span class="sxs-lookup"><span data-stu-id="15372-106">You can specify a specific drive or site, display a list of files based on insight type (trending, used, or shared), or provide queries to a custom list of files.</span></span>

## <a name="example"></a><span data-ttu-id="15372-107">Пример</span><span class="sxs-lookup"><span data-stu-id="15372-107">Example</span></span>

<span data-ttu-id="15372-108">В следующем примере отображается файл с помощью `mgt-file-list` компонента.</span><span class="sxs-lookup"><span data-stu-id="15372-108">The following example displays a file using the `mgt-file-list` component.</span></span> <span data-ttu-id="15372-109">Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="15372-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-file-list--file-list&source=docs" height="250"></iframe>

[<span data-ttu-id="15372-110">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="15372-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-file-list--file-list&source=docs)

## <a name="properties"></a><span data-ttu-id="15372-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="15372-111">Properties</span></span>

<span data-ttu-id="15372-112">Для настройки компонента можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="15372-112">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="15372-113">Атрибут</span><span class="sxs-lookup"><span data-stu-id="15372-113">Attribute</span></span> | <span data-ttu-id="15372-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="15372-114">Property</span></span> | <span data-ttu-id="15372-115">Описание</span><span class="sxs-lookup"><span data-stu-id="15372-115">Description</span></span> |
| --------- | -------- | ----------- |
| <span data-ttu-id="15372-116">файл-список-запрос</span><span class="sxs-lookup"><span data-stu-id="15372-116">file-list-query</span></span> | <span data-ttu-id="15372-117">fileListQuery</span><span class="sxs-lookup"><span data-stu-id="15372-117">fileListQuery</span></span> | <span data-ttu-id="15372-118">Полный запрос или путь к диску или сайту, содержащий список отрисовки файлов.</span><span class="sxs-lookup"><span data-stu-id="15372-118">The full query or path to the drive or site that contains the list of files to render.</span></span> |
| <span data-ttu-id="15372-119">файл-запросы</span><span class="sxs-lookup"><span data-stu-id="15372-119">file-queries</span></span> | <span data-ttu-id="15372-120">fileQueries</span><span class="sxs-lookup"><span data-stu-id="15372-120">fileQueries</span></span> | <span data-ttu-id="15372-121">Массив файлового запроса, отрисовываемого компонентом.</span><span class="sxs-lookup"><span data-stu-id="15372-121">An array of file queries to be rendered by the component.</span></span> |
| <span data-ttu-id="15372-122">нет</span><span class="sxs-lookup"><span data-stu-id="15372-122">none</span></span> | <span data-ttu-id="15372-123">files</span><span class="sxs-lookup"><span data-stu-id="15372-123">files</span></span> | <span data-ttu-id="15372-124">Массив файлов для получения или набора списка файлов, отрисовываний компонентом.</span><span class="sxs-lookup"><span data-stu-id="15372-124">An array of files to get or set the list of files rendered by the component.</span></span> <span data-ttu-id="15372-125">Используйте это для доступа к файлам, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="15372-125">Use this to access the files loaded by the component.</span></span> <span data-ttu-id="15372-126">Установите это значение для загрузки собственных файлов.</span><span class="sxs-lookup"><span data-stu-id="15372-126">Set this value to load your own files.</span></span> |
| <span data-ttu-id="15372-127">тип insight</span><span class="sxs-lookup"><span data-stu-id="15372-127">insight-type</span></span> | <span data-ttu-id="15372-128">insightType</span><span class="sxs-lookup"><span data-stu-id="15372-128">insightType</span></span> | <span data-ttu-id="15372-129">Установите для демонстрации трендовых, используемых или общих файлов пользователя.</span><span class="sxs-lookup"><span data-stu-id="15372-129">Set to show the user’s trending, used, or shared files.</span></span> |
| <span data-ttu-id="15372-130">drive-id</span><span class="sxs-lookup"><span data-stu-id="15372-130">drive-id</span></span> | <span data-ttu-id="15372-131">driveId</span><span class="sxs-lookup"><span data-stu-id="15372-131">driveId</span></span> | <span data-ttu-id="15372-132">ID диска, к которой принадлежит папка.</span><span class="sxs-lookup"><span data-stu-id="15372-132">ID of the drive the folder belongs to.</span></span> <span data-ttu-id="15372-133">Также необходимо предоставить либо `item-id` `item-path` .</span><span class="sxs-lookup"><span data-stu-id="15372-133">Must also provide either `item-id` or `item-path`.</span></span> |
| <span data-ttu-id="15372-134">group-id</span><span class="sxs-lookup"><span data-stu-id="15372-134">group-id</span></span> | <span data-ttu-id="15372-135">groupId</span><span class="sxs-lookup"><span data-stu-id="15372-135">groupId</span></span> | <span data-ttu-id="15372-136">ID группы, которой принадлежит папка.</span><span class="sxs-lookup"><span data-stu-id="15372-136">ID of the group the folder belongs to.</span></span> <span data-ttu-id="15372-137">Также необходимо предоставить либо `item-id` `item-path` .</span><span class="sxs-lookup"><span data-stu-id="15372-137">Must also provide either `item-id` or `item-path`.</span></span> |
| <span data-ttu-id="15372-138">site-id</span><span class="sxs-lookup"><span data-stu-id="15372-138">site-id</span></span> | <span data-ttu-id="15372-139">siteId</span><span class="sxs-lookup"><span data-stu-id="15372-139">siteId</span></span> | <span data-ttu-id="15372-140">ID сайта, к которой принадлежит папка.</span><span class="sxs-lookup"><span data-stu-id="15372-140">ID of the site the folder belongs to.</span></span> <span data-ttu-id="15372-141">Также необходимо предоставить либо `{item-id}` `{item-path}` .</span><span class="sxs-lookup"><span data-stu-id="15372-141">Must also provide either `{item-id}` or `{item-path}`.</span></span> <span data-ttu-id="15372-142">`{list-id}`Укай, если вы ссылаетесь на файл из определенного списка.</span><span class="sxs-lookup"><span data-stu-id="15372-142">Provide `{list-id}` if you’re referencing a file from a specific list.</span></span> |
| <span data-ttu-id="15372-143">item-id</span><span class="sxs-lookup"><span data-stu-id="15372-143">item-id</span></span> | <span data-ttu-id="15372-144">itemId</span><span class="sxs-lookup"><span data-stu-id="15372-144">itemId</span></span> | <span data-ttu-id="15372-145">ID папки.</span><span class="sxs-lookup"><span data-stu-id="15372-145">ID of the folder.</span></span> <span data-ttu-id="15372-146">Запрос по умолчанию `/me/drive/items` .</span><span class="sxs-lookup"><span data-stu-id="15372-146">Default query is `/me/drive/items`.</span></span> <span data-ttu-id="15372-147">Предоставление `{drive-id}` , или запрос `{group-id}` `{site-id}` `{user-id}` определенного расположения.</span><span class="sxs-lookup"><span data-stu-id="15372-147">Provide `{drive-id}`, `{group-id}`, `{site-id}`, or `{user-id}` to query a specific location.</span></span> |
| <span data-ttu-id="15372-148">путь элемента</span><span class="sxs-lookup"><span data-stu-id="15372-148">item-path</span></span> | <span data-ttu-id="15372-149">itemPath</span><span class="sxs-lookup"><span data-stu-id="15372-149">itemPath</span></span> | <span data-ttu-id="15372-150">Путь элемента папки (относительно корневого).</span><span class="sxs-lookup"><span data-stu-id="15372-150">Item path of the folder (relative to the root).</span></span> <span data-ttu-id="15372-151">Запрос по умолчанию `/me/drive/root` .</span><span class="sxs-lookup"><span data-stu-id="15372-151">Default query is `/me/drive/root`.</span></span> <span data-ttu-id="15372-152">Предоставление `{drive-id}` , или запрос `{group-id}` `{site-id}` `{user-id}` определенного расположения.</span><span class="sxs-lookup"><span data-stu-id="15372-152">Provide `{drive-id}`, `{group-id}`, `{site-id}`, or `{user-id}` to query a specific location.</span></span> |
| <span data-ttu-id="15372-153">размер страницы</span><span class="sxs-lookup"><span data-stu-id="15372-153">page-size</span></span> | <span data-ttu-id="15372-154">pageSize</span><span class="sxs-lookup"><span data-stu-id="15372-154">pageSize</span></span> | <span data-ttu-id="15372-155">Значение числа, чтобы указать максимальное количество файлов, которые необходимо отрисовки на каждой странице.</span><span class="sxs-lookup"><span data-stu-id="15372-155">A number value to indicate the maximum number of files to render on each page.</span></span> |
| <span data-ttu-id="15372-156">расширения файлов</span><span class="sxs-lookup"><span data-stu-id="15372-156">file-extensions</span></span> | <span data-ttu-id="15372-157">fileExtensions</span><span class="sxs-lookup"><span data-stu-id="15372-157">fileExtensions</span></span> | <span data-ttu-id="15372-158">Массив расширений файлов, используемых для фильтрации файлов для показа.</span><span class="sxs-lookup"><span data-stu-id="15372-158">An array of file extensions used to filter files to show.</span></span> |
| <span data-ttu-id="15372-159">кнопка hide-more-files-button</span><span class="sxs-lookup"><span data-stu-id="15372-159">hide-more-files-button</span></span> | <span data-ttu-id="15372-160">hideMoreFilesButton</span><span class="sxs-lookup"><span data-stu-id="15372-160">hideMoreFilesButton</span></span> | <span data-ttu-id="15372-161">A boolean to indicate whether to show a button to render more files.</span><span class="sxs-lookup"><span data-stu-id="15372-161">A boolean to indicate whether to show a button to render more files.</span></span> |

<span data-ttu-id="15372-162">В следующем примере изменяется поведение компонента для получения списка файлов из определенного запроса.</span><span class="sxs-lookup"><span data-stu-id="15372-162">The following example changes the behavior of the component to fetch a file list from a specific query.</span></span>

```html
<mgt-file-list file-list-query="/me/drive/items/01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY/children"></mgt-file-list>
```

<span data-ttu-id="15372-163">В следующем примере изменяется поведение компонента для получения списка файлов из папки, предоставляя id папки.</span><span class="sxs-lookup"><span data-stu-id="15372-163">The following example changes the behavior of the component to fetch a file list from a folder by providing the folder id.</span></span>

```html
<mgt-file-list item-id="01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY"></mgt-file-list>
```

<span data-ttu-id="15372-164">В следующем примере изменяется поведение компонента для получения списка файлов из группы, предоставляя групповой id и путь папки.</span><span class="sxs-lookup"><span data-stu-id="15372-164">The following example changes the behavior of the component to fetch file list from a group by providing the group id and folder path.</span></span>

```html
<mgt-file-list group-id="8090c93e-ba7c-433e-9f39-08c7ba07c0b3" item-path="/Design"></mgt-file-list>
```

<span data-ttu-id="15372-165">В следующем примере изменяется поведение компонента для получения списка файлов от пользователя, предоставляя пользовательский ид папки.</span><span class="sxs-lookup"><span data-stu-id="15372-165">The following example changes the behavior of the component to fetch file list from a user by providing the user id and folder id.</span></span>

```html
<mgt-file-list user-id="48d31887-5fad-4d73-a9f5-3c356e68a038" item-id="01BYE5RZYFPM65IDVARFELFLNTXR4ZKABD"></mgt-file-list>
```

<span data-ttu-id="15372-166">В следующем примере изменяется поведение компонента для получения списка файлов, предоставляя тип проницательности.</span><span class="sxs-lookup"><span data-stu-id="15372-166">The following example changes the behavior of the component to fetch file list by providing the insight type.</span></span>

```html
<mgt-file-list insight-type="shared"></mgt-file-list>
```

## <a name="css-custom-properties"></a><span data-ttu-id="15372-167">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="15372-167">CSS custom properties</span></span>

<span data-ttu-id="15372-168">Компонент `mgt-file-list` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="15372-168">The `mgt-file-list` component defines the following CSS custom properties.</span></span>

```css
mgt-file-list {
  --font-family: 'Segoe UI';
  --font-size: 14px;

  --file-list-background-color: #ffffff;
  --file-list-border: none;
  --file-list-box-shadow: none;
  --file-list-padding: 4px 0;
  --file-list-margin: 0;

  --file-item-background-color--hover: rgba(0, 0, 0, 0.1);
  --file-item-background-color--active: rgba(0, 0, 0, 0.05);
  --file-item-border-radius: 2px;
  --file-item-margin: 0 4px;

  --file-item-border-top: none;
  --file-item-border-left: none;
  --file-item-border-right: none;
  --file-item-border-bottom: none;

  --show-more-button-background-color: #f3f2f1;
  --show-more-button-background-color--hover: rgba(0, 0, 0, 0.1);
  --show-more-button-font-size: 12px;
  --show-more-button-padding: 6px;
  --show-more-button-border-bottom-right-radius: 4px;
  --show-more-button-border-bottom-left-radius: 4px;
}
```

<span data-ttu-id="15372-169">Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="15372-169">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="microsoft-graph-apis-and-permissions"></a><span data-ttu-id="15372-170">Страница "Разрешения API и приложений Microsoft Graph"</span><span class="sxs-lookup"><span data-stu-id="15372-170">Microsoft Graph APIs and permissions</span></span>

| <span data-ttu-id="15372-171">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="15372-171">Configuration</span></span> | <span data-ttu-id="15372-172">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15372-172">Permissions</span></span> | <span data-ttu-id="15372-173">API</span><span class="sxs-lookup"><span data-stu-id="15372-173">API</span></span> |
| ------------- | ----------------- | --- |
| <span data-ttu-id="15372-174">По умолчанию (не предоставлены идентификаторы или запросы)</span><span class="sxs-lookup"><span data-stu-id="15372-174">Default (no identifiers or query provided)</span></span> | <span data-ttu-id="15372-175">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-175">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/root/children`   |
| <span data-ttu-id="15372-176">Предоставление `{drive-id}` И `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="15372-176">Provide `{drive-id}` AND `{item-id}`</span></span> | <span data-ttu-id="15372-177">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-177">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /drives/{drive-id}/items/{item-id}/children` |
| <span data-ttu-id="15372-178">Предоставление `{group-id}` И `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="15372-178">Provide `{group-id}` AND `{item-id}`</span></span> | <span data-ttu-id="15372-179">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-179">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /groups/{group-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="15372-180">Предоставление ТОЛЬКО `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="15372-180">Provide ONLY `{item-id}`</span></span> | <span data-ttu-id="15372-181">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-181">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/items/{item-id}/children` | 
| <span data-ttu-id="15372-182">Предоставление `{site-id}` И `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="15372-182">Provide `{site-id}` AND `{item-id}`</span></span> | <span data-ttu-id="15372-183">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-183">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="15372-184">Pprovide `{user-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="15372-184">Pprovide `{user-id}` AND `{item-id}`</span></span> | <span data-ttu-id="15372-185">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-185">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /users/{user-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="15372-186">Предоставление `{drive-id}` И `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="15372-186">Provide `{drive-id}` AND `{item-path}`</span></span> | <span data-ttu-id="15372-187">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-187">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /drives/{drive-id}/root:/{item-path}:/children` |
| <span data-ttu-id="15372-188">Предоставление `{group-id}` И `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="15372-188">Provide `{group-id}` AND `{item-path}`</span></span> | <span data-ttu-id="15372-189">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-189">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /groups/{group-id}/root:/{item-path}:/children` |
| <span data-ttu-id="15372-190">Предоставление `{site-id}` И `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="15372-190">Provide `{site-id}` AND `{item-path}`</span></span> | <span data-ttu-id="15372-191">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-191">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/root:/{item-path}:/children` |
| <span data-ttu-id="15372-192">Предоставление `{user-id}` И `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="15372-192">Provide `{user-id}` AND `{item-path}`</span></span> | <span data-ttu-id="15372-193">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-193">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /users/{user-id}/root:/{item-path}:/children` |
| <span data-ttu-id="15372-194">Предоставление только `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="15372-194">Provide only `{item-path}`</span></span> | <span data-ttu-id="15372-195">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-195">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/root:/{item-path}:/children` |
| <span data-ttu-id="15372-196">`insight-type` настроена на трендовую</span><span class="sxs-lookup"><span data-stu-id="15372-196">`insight-type` is set to trending</span></span> | <span data-ttu-id="15372-197">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-197">Sites.Read.All</span></span> | `GET /me/insights/trending` |
| <span data-ttu-id="15372-198">Обеспечить `{user-id or upn}` и `insight-type` установить для `trending`</span><span class="sxs-lookup"><span data-stu-id="15372-198">Provide `{user-id or upn}` AND `insight-type` is set to `trending`</span></span> | <span data-ttu-id="15372-199">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-199">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/trending` | 
| <span data-ttu-id="15372-200">`insight-type` установлено, что `used`</span><span class="sxs-lookup"><span data-stu-id="15372-200">`insight-type` is set to `used`</span></span> | <span data-ttu-id="15372-201">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-201">Sites.Read.All</span></span> | `GET /me/insights/used` |
| <span data-ttu-id="15372-202">Обеспечить `{user-id or upn}` и `insight-type` установить для `used`</span><span class="sxs-lookup"><span data-stu-id="15372-202">Provide `{user-id or upn}` AND `insight-type` is set to `used`</span></span> | <span data-ttu-id="15372-203">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-203">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/used` |
| <span data-ttu-id="15372-204">`insight-type` настроено на общий доступ</span><span class="sxs-lookup"><span data-stu-id="15372-204">`insight-type` is set to shared</span></span> | <span data-ttu-id="15372-205">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-205">Sites.Read.All</span></span> | `GET /me/insights/shared` |
| <span data-ttu-id="15372-206">Обеспечить `{user-id or upn}` и `insight-type` установить для `shared`</span><span class="sxs-lookup"><span data-stu-id="15372-206">Provide `{user-id or upn}` AND `insight-type` is set to `shared`</span></span> | <span data-ttu-id="15372-207">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="15372-207">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/shared?$filter=((lastshared/sharedby/id eq '${user-id}') and (resourceReference/type eq 'microsoft.graph.driveItem'))` |

## <a name="events"></a><span data-ttu-id="15372-208">События</span><span class="sxs-lookup"><span data-stu-id="15372-208">Events</span></span>

| <span data-ttu-id="15372-209">Событие</span><span class="sxs-lookup"><span data-stu-id="15372-209">Event</span></span> | <span data-ttu-id="15372-210">Описание</span><span class="sxs-lookup"><span data-stu-id="15372-210">Description</span></span> |
| ----- | ----------- |
| <span data-ttu-id="15372-211">itemClick</span><span class="sxs-lookup"><span data-stu-id="15372-211">itemClick</span></span> | <span data-ttu-id="15372-212">Уволили, когда пользователь щелкнуть файл.</span><span class="sxs-lookup"><span data-stu-id="15372-212">Fired when the user clicks a file.</span></span> <span data-ttu-id="15372-213">Возвращает сведения о файле.</span><span class="sxs-lookup"><span data-stu-id="15372-213">Returns the file details.</span></span> |

## <a name="templates"></a><span data-ttu-id="15372-214">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="15372-214">Templates</span></span>

<span data-ttu-id="15372-215">Компонент `mgt-file-list` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="15372-215">The `mgt-file-list` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="15372-216">Чтобы указать шаблон, включи элемент внутри компонента и закажите значение для одного из типов данных, перечисленных `<template>` `data-type` в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="15372-216">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the data types listed in the following table.</span></span>

| <span data-ttu-id="15372-217">Тип данных</span><span class="sxs-lookup"><span data-stu-id="15372-217">Data type</span></span> | <span data-ttu-id="15372-218">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="15372-218">Data context</span></span> | <span data-ttu-id="15372-219">Описание</span><span class="sxs-lookup"><span data-stu-id="15372-219">Description</span></span> |
| ----------- | -------------- | ------------ |
| <span data-ttu-id="15372-220">default</span><span class="sxs-lookup"><span data-stu-id="15372-220">default</span></span> | <span data-ttu-id="15372-221">`files`: список объектов файлов</span><span class="sxs-lookup"><span data-stu-id="15372-221">`files`: list of file objects</span></span> | <span data-ttu-id="15372-222">Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом.</span><span class="sxs-lookup"><span data-stu-id="15372-222">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="15372-223">file</span><span class="sxs-lookup"><span data-stu-id="15372-223">file</span></span> | <span data-ttu-id="15372-224">`file`: объект файла</span><span class="sxs-lookup"><span data-stu-id="15372-224">`file`: file object</span></span> | <span data-ttu-id="15372-225">Шаблон, используемый для отрисовки каждого файла.</span><span class="sxs-lookup"><span data-stu-id="15372-225">The template used to render each file.</span></span> |
| <span data-ttu-id="15372-226">no-data</span><span class="sxs-lookup"><span data-stu-id="15372-226">no-data</span></span> | <span data-ttu-id="15372-227">Контекст данных не передан</span><span class="sxs-lookup"><span data-stu-id="15372-227">No data context is passed</span></span> | <span data-ttu-id="15372-228">Шаблон, используемый, если данные недоступны.</span><span class="sxs-lookup"><span data-stu-id="15372-228">The template used when no data is available.</span></span> |
| <span data-ttu-id="15372-229">loading</span><span class="sxs-lookup"><span data-stu-id="15372-229">loading</span></span> | <span data-ttu-id="15372-230">Контекст данных не передан</span><span class="sxs-lookup"><span data-stu-id="15372-230">No data context is passed</span></span> | <span data-ttu-id="15372-231">Шаблон, используемый при загрузке состояния компонента.</span><span class="sxs-lookup"><span data-stu-id="15372-231">The template used while the component loads state.</span></span> |

## <a name="authentication"></a><span data-ttu-id="15372-232">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="15372-232">Authentication</span></span>

<span data-ttu-id="15372-233">Для получения требуемых данных в средстве управления используется глобальный поставщик проверки подлинности, указанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="15372-233">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="cache"></a><span data-ttu-id="15372-234">Кэш</span><span class="sxs-lookup"><span data-stu-id="15372-234">Cache</span></span>

|<span data-ttu-id="15372-235">Хранилище объектов</span><span class="sxs-lookup"><span data-stu-id="15372-235">Object store</span></span>|<span data-ttu-id="15372-236">Кэшные данные</span><span class="sxs-lookup"><span data-stu-id="15372-236">Cached data</span></span>|<span data-ttu-id="15372-237">Примечания</span><span class="sxs-lookup"><span data-stu-id="15372-237">Remarks</span></span>|
|---------|-----------|-------|
|`fileLists`|<span data-ttu-id="15372-238">Список списков файлов</span><span class="sxs-lookup"><span data-stu-id="15372-238">List of file lists</span></span>|<span data-ttu-id="15372-239">Список кэша по умолчанию для хранения списков файлов.</span><span class="sxs-lookup"><span data-stu-id="15372-239">Default cache list to store file lists.</span></span>|
|`insightfileLists`|<span data-ttu-id="15372-240">Список списков файлов анализа</span><span class="sxs-lookup"><span data-stu-id="15372-240">List of insight file lists</span></span>|<span data-ttu-id="15372-241">Используется при `insightType` условии.</span><span class="sxs-lookup"><span data-stu-id="15372-241">Used when `insightType` is provided.</span></span>|

> [!NOTE]
> <span data-ttu-id="15372-242">Компонент `mgt-file-list` также использует хранилище объектов в IndexedDB для `fileQueries` `mgt-file` кэша файлов при `fileQueries` условии.</span><span class="sxs-lookup"><span data-stu-id="15372-242">The `mgt-file-list` component also uses the `fileQueries` object store in `mgt-file` IndexedDB to cache files when `fileQueries` is provided.</span></span>

<span data-ttu-id="15372-243">Сведения о настройке кэша см. в материале [Caching.](../customize-components/cache.md)</span><span class="sxs-lookup"><span data-stu-id="15372-243">For details about how to configure the cache, see [Caching](../customize-components/cache.md).</span></span>