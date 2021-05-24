---
title: Компонент списка файлов в microsoft Graph набор средств
description: Компонент списка файлов используется для отображения списка файлов, показывая их значок и имя
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: bde548e843170de6cd1234f14096339859d4b99b
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629170"
---
# <a name="file-list-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="4f7f4-103">Компонент списка файлов в microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="4f7f4-103">File list component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="4f7f4-104">Компонент Списка файлов [](/graph/api/resources/onedrive) отображает список нескольких папок и файлов с помощью имени файла или папки, значка и других свойств, которые вы указываете.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-104">The File List component displays [a list of multiple folders and files](/graph/api/resources/onedrive) by using the file/folder name, an icon, and other properties that you specify.</span></span> <span data-ttu-id="4f7f4-105">Этот компонент использует [компонент mgt-file.](./file.md)</span><span class="sxs-lookup"><span data-stu-id="4f7f4-105">This component uses the [mgt-file](./file.md) component.</span></span> <span data-ttu-id="4f7f4-106">Вы можете указать определенный диск или сайт, отобразить список файлов, основанный на типе insight (трендовые, используемые или общие), или предоставить запросы в настраиваемый список файлов.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-106">You can specify a specific drive or site, display a list of files based on insight type (trending, used, or shared), or provide queries to a custom list of files.</span></span>

## <a name="example"></a><span data-ttu-id="4f7f4-107">Пример</span><span class="sxs-lookup"><span data-stu-id="4f7f4-107">Example</span></span>

<span data-ttu-id="4f7f4-108">В следующем примере отображается файл с помощью `mgt-file-list` компонента.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-108">The following example displays a file using the `mgt-file-list` component.</span></span> <span data-ttu-id="4f7f4-109">Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-file-list--file-list&source=docs" height="250"></iframe>

[<span data-ttu-id="4f7f4-110">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="4f7f4-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-file-list--file-list&source=docs)

## <a name="properties"></a><span data-ttu-id="4f7f4-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f7f4-111">Properties</span></span>

<span data-ttu-id="4f7f4-112">Для настройки компонента можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-112">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="4f7f4-113">Атрибут</span><span class="sxs-lookup"><span data-stu-id="4f7f4-113">Attribute</span></span> | <span data-ttu-id="4f7f4-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f7f4-114">Property</span></span> | <span data-ttu-id="4f7f4-115">Описание</span><span class="sxs-lookup"><span data-stu-id="4f7f4-115">Description</span></span> |
| --------- | -------- | ----------- |
| <span data-ttu-id="4f7f4-116">файл-список-запрос</span><span class="sxs-lookup"><span data-stu-id="4f7f4-116">file-list-query</span></span> | <span data-ttu-id="4f7f4-117">fileListQuery</span><span class="sxs-lookup"><span data-stu-id="4f7f4-117">fileListQuery</span></span> | <span data-ttu-id="4f7f4-118">Полный запрос или путь к диску или сайту, содержащий список отрисовки файлов.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-118">The full query or path to the drive or site that contains the list of files to render.</span></span> |
| <span data-ttu-id="4f7f4-119">файл-запросы</span><span class="sxs-lookup"><span data-stu-id="4f7f4-119">file-queries</span></span> | <span data-ttu-id="4f7f4-120">fileQueries</span><span class="sxs-lookup"><span data-stu-id="4f7f4-120">fileQueries</span></span> | <span data-ttu-id="4f7f4-121">Массив файлового запроса, отрисовываемого компонентом.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-121">An array of file queries to be rendered by the component.</span></span> |
| <span data-ttu-id="4f7f4-122">нет</span><span class="sxs-lookup"><span data-stu-id="4f7f4-122">none</span></span> | <span data-ttu-id="4f7f4-123">files</span><span class="sxs-lookup"><span data-stu-id="4f7f4-123">files</span></span> | <span data-ttu-id="4f7f4-124">Массив файлов для получения или набора списка файлов, отрисовываний компонентом.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-124">An array of files to get or set the list of files rendered by the component.</span></span> <span data-ttu-id="4f7f4-125">Используйте это для доступа к файлам, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-125">Use this to access the files loaded by the component.</span></span> <span data-ttu-id="4f7f4-126">Установите это значение для загрузки собственных файлов.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-126">Set this value to load your own files.</span></span> |
| <span data-ttu-id="4f7f4-127">тип insight</span><span class="sxs-lookup"><span data-stu-id="4f7f4-127">insight-type</span></span> | <span data-ttu-id="4f7f4-128">insightType</span><span class="sxs-lookup"><span data-stu-id="4f7f4-128">insightType</span></span> | <span data-ttu-id="4f7f4-129">Установите для демонстрации трендовых, используемых или общих файлов пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-129">Set to show the user’s trending, used, or shared files.</span></span> |
| <span data-ttu-id="4f7f4-130">drive-id</span><span class="sxs-lookup"><span data-stu-id="4f7f4-130">drive-id</span></span> | <span data-ttu-id="4f7f4-131">driveId</span><span class="sxs-lookup"><span data-stu-id="4f7f4-131">driveId</span></span> | <span data-ttu-id="4f7f4-132">ID диска, к которой принадлежит папка.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-132">ID of the drive the folder belongs to.</span></span> <span data-ttu-id="4f7f4-133">Также необходимо предоставить либо `item-id` `item-path` .</span><span class="sxs-lookup"><span data-stu-id="4f7f4-133">Must also provide either `item-id` or `item-path`.</span></span> |
| <span data-ttu-id="4f7f4-134">group-id</span><span class="sxs-lookup"><span data-stu-id="4f7f4-134">group-id</span></span> | <span data-ttu-id="4f7f4-135">groupId</span><span class="sxs-lookup"><span data-stu-id="4f7f4-135">groupId</span></span> | <span data-ttu-id="4f7f4-136">ID группы, которой принадлежит папка.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-136">ID of the group the folder belongs to.</span></span> <span data-ttu-id="4f7f4-137">Также необходимо предоставить либо `item-id` `item-path` .</span><span class="sxs-lookup"><span data-stu-id="4f7f4-137">Must also provide either `item-id` or `item-path`.</span></span> |
| <span data-ttu-id="4f7f4-138">site-id</span><span class="sxs-lookup"><span data-stu-id="4f7f4-138">site-id</span></span> | <span data-ttu-id="4f7f4-139">siteId</span><span class="sxs-lookup"><span data-stu-id="4f7f4-139">siteId</span></span> | <span data-ttu-id="4f7f4-140">ID сайта, к которой принадлежит папка.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-140">ID of the site the folder belongs to.</span></span> <span data-ttu-id="4f7f4-141">Также необходимо предоставить либо `{item-id}` `{item-path}` .</span><span class="sxs-lookup"><span data-stu-id="4f7f4-141">Must also provide either `{item-id}` or `{item-path}`.</span></span> <span data-ttu-id="4f7f4-142">`{list-id}`Укай, если вы ссылаетесь на файл из определенного списка.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-142">Provide `{list-id}` if you’re referencing a file from a specific list.</span></span> |
| <span data-ttu-id="4f7f4-143">item-id</span><span class="sxs-lookup"><span data-stu-id="4f7f4-143">item-id</span></span> | <span data-ttu-id="4f7f4-144">itemId</span><span class="sxs-lookup"><span data-stu-id="4f7f4-144">itemId</span></span> | <span data-ttu-id="4f7f4-145">ID папки.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-145">ID of the folder.</span></span> <span data-ttu-id="4f7f4-146">Запрос по умолчанию `/me/drive/items` .</span><span class="sxs-lookup"><span data-stu-id="4f7f4-146">Default query is `/me/drive/items`.</span></span> <span data-ttu-id="4f7f4-147">Предоставление `{drive-id}` , или запрос `{group-id}` `{site-id}` `{user-id}` определенного расположения.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-147">Provide `{drive-id}`, `{group-id}`, `{site-id}`, or `{user-id}` to query a specific location.</span></span> |
| <span data-ttu-id="4f7f4-148">путь элемента</span><span class="sxs-lookup"><span data-stu-id="4f7f4-148">item-path</span></span> | <span data-ttu-id="4f7f4-149">itemPath</span><span class="sxs-lookup"><span data-stu-id="4f7f4-149">itemPath</span></span> | <span data-ttu-id="4f7f4-150">Путь элемента папки (относительно корневого).</span><span class="sxs-lookup"><span data-stu-id="4f7f4-150">Item path of the folder (relative to the root).</span></span> <span data-ttu-id="4f7f4-151">Запрос по умолчанию `/me/drive/root` .</span><span class="sxs-lookup"><span data-stu-id="4f7f4-151">Default query is `/me/drive/root`.</span></span> <span data-ttu-id="4f7f4-152">Предоставление `{drive-id}` , или запрос `{group-id}` `{site-id}` `{user-id}` определенного расположения.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-152">Provide `{drive-id}`, `{group-id}`, `{site-id}`, or `{user-id}` to query a specific location.</span></span> |
| <span data-ttu-id="4f7f4-153">размер страницы</span><span class="sxs-lookup"><span data-stu-id="4f7f4-153">page-size</span></span> | <span data-ttu-id="4f7f4-154">pageSize</span><span class="sxs-lookup"><span data-stu-id="4f7f4-154">pageSize</span></span> | <span data-ttu-id="4f7f4-155">Значение числа, чтобы указать максимальное количество файлов, которые необходимо отрисовки на каждой странице.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-155">A number value to indicate the maximum number of files to render on each page.</span></span> |
| <span data-ttu-id="4f7f4-156">расширения файлов</span><span class="sxs-lookup"><span data-stu-id="4f7f4-156">file-extensions</span></span> | <span data-ttu-id="4f7f4-157">fileExtensions</span><span class="sxs-lookup"><span data-stu-id="4f7f4-157">fileExtensions</span></span> | <span data-ttu-id="4f7f4-158">Массив расширений файлов, используемых для фильтрации файлов для показа.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-158">An array of file extensions used to filter files to show.</span></span> |
| <span data-ttu-id="4f7f4-159">кнопка hide-more-files-button</span><span class="sxs-lookup"><span data-stu-id="4f7f4-159">hide-more-files-button</span></span> | <span data-ttu-id="4f7f4-160">hideMoreFilesButton</span><span class="sxs-lookup"><span data-stu-id="4f7f4-160">hideMoreFilesButton</span></span> | <span data-ttu-id="4f7f4-161">A boolean to indicate whether to show a button to render more files.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-161">A boolean to indicate whether to show a button to render more files.</span></span> |

<span data-ttu-id="4f7f4-162">В следующем примере изменяется поведение компонента для получения списка файлов из определенного запроса.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-162">The following example changes the behavior of the component to fetch a file list from a specific query.</span></span>

```html
<mgt-file-list file-list-query="/me/drive/items/01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY/children"></mgt-file-list>
```

<span data-ttu-id="4f7f4-163">В следующем примере изменяется поведение компонента для получения списка файлов из папки, предоставляя id папки.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-163">The following example changes the behavior of the component to fetch a file list from a folder by providing the folder id.</span></span>

```html
<mgt-file-list item-id="01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY"></mgt-file-list>
```

<span data-ttu-id="4f7f4-164">В следующем примере изменяется поведение компонента для получения списка файлов из группы, предоставляя групповой id и путь папки.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-164">The following example changes the behavior of the component to fetch file list from a group by providing the group id and folder path.</span></span>

```html
<mgt-file-list group-id="8090c93e-ba7c-433e-9f39-08c7ba07c0b3" item-path="/Design"></mgt-file-list>
```

<span data-ttu-id="4f7f4-165">В следующем примере изменяется поведение компонента для получения списка файлов от пользователя, предоставляя пользовательский ид папки.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-165">The following example changes the behavior of the component to fetch file list from a user by providing the user id and folder id.</span></span>

```html
<mgt-file-list user-id="48d31887-5fad-4d73-a9f5-3c356e68a038" item-id="01BYE5RZYFPM65IDVARFELFLNTXR4ZKABD"></mgt-file-list>
```

<span data-ttu-id="4f7f4-166">В следующем примере изменяется поведение компонента для получения списка файлов, предоставляя тип проницательности.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-166">The following example changes the behavior of the component to fetch file list by providing the insight type.</span></span>

```html
<mgt-file-list insight-type="shared"></mgt-file-list>
```

## <a name="methods"></a><span data-ttu-id="4f7f4-167">Методы</span><span class="sxs-lookup"><span data-stu-id="4f7f4-167">Methods</span></span>
| <span data-ttu-id="4f7f4-168">Метод</span><span class="sxs-lookup"><span data-stu-id="4f7f4-168">Method</span></span> | <span data-ttu-id="4f7f4-169">Описание</span><span class="sxs-lookup"><span data-stu-id="4f7f4-169">Description</span></span> |
| --- | --- |
| <span data-ttu-id="4f7f4-170">перезагрузка (clearCache = false)</span><span class="sxs-lookup"><span data-stu-id="4f7f4-170">reload(clearCache = false)</span></span> | <span data-ttu-id="4f7f4-171">Вызывает метод для перезагрузки компонента с потенциальными новыми данными на основе его свойств.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-171">Call the method to reload the component with potential new data based on its properties.</span></span> <span data-ttu-id="4f7f4-172">Перед перезагрузки необходимо очистить `true` кэш.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-172">Pass `true` to clear the cache before reloading.</span></span> |

## <a name="css-custom-properties"></a><span data-ttu-id="4f7f4-173">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="4f7f4-173">CSS custom properties</span></span>

<span data-ttu-id="4f7f4-174">Компонент `mgt-file-list` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-174">The `mgt-file-list` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="4f7f4-175">Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="4f7f4-175">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="microsoft-graph-apis-and-permissions"></a><span data-ttu-id="4f7f4-176">Страница "Разрешения API и приложений Microsoft Graph"</span><span class="sxs-lookup"><span data-stu-id="4f7f4-176">Microsoft Graph APIs and permissions</span></span>

| <span data-ttu-id="4f7f4-177">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="4f7f4-177">Configuration</span></span> | <span data-ttu-id="4f7f4-178">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f7f4-178">Permissions</span></span> | <span data-ttu-id="4f7f4-179">API</span><span class="sxs-lookup"><span data-stu-id="4f7f4-179">API</span></span> |
| ------------- | ----------------- | --- |
| <span data-ttu-id="4f7f4-180">По умолчанию (не предоставлены идентификаторы или запросы)</span><span class="sxs-lookup"><span data-stu-id="4f7f4-180">Default (no identifiers or query provided)</span></span> | <span data-ttu-id="4f7f4-181">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-181">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/root/children`   |
| <span data-ttu-id="4f7f4-182">Предоставление `{drive-id}` И `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="4f7f4-182">Provide `{drive-id}` AND `{item-id}`</span></span> | <span data-ttu-id="4f7f4-183">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-183">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /drives/{drive-id}/items/{item-id}/children` |
| <span data-ttu-id="4f7f4-184">Предоставление `{group-id}` И `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="4f7f4-184">Provide `{group-id}` AND `{item-id}`</span></span> | <span data-ttu-id="4f7f4-185">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-185">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /groups/{group-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="4f7f4-186">Предоставление ТОЛЬКО `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="4f7f4-186">Provide ONLY `{item-id}`</span></span> | <span data-ttu-id="4f7f4-187">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-187">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/items/{item-id}/children` | 
| <span data-ttu-id="4f7f4-188">Предоставление `{site-id}` И `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="4f7f4-188">Provide `{site-id}` AND `{item-id}`</span></span> | <span data-ttu-id="4f7f4-189">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-189">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="4f7f4-190">Pprovide `{user-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="4f7f4-190">Pprovide `{user-id}` AND `{item-id}`</span></span> | <span data-ttu-id="4f7f4-191">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-191">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /users/{user-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="4f7f4-192">Предоставление `{drive-id}` И `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="4f7f4-192">Provide `{drive-id}` AND `{item-path}`</span></span> | <span data-ttu-id="4f7f4-193">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-193">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /drives/{drive-id}/root:/{item-path}:/children` |
| <span data-ttu-id="4f7f4-194">Предоставление `{group-id}` И `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="4f7f4-194">Provide `{group-id}` AND `{item-path}`</span></span> | <span data-ttu-id="4f7f4-195">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-195">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /groups/{group-id}/root:/{item-path}:/children` |
| <span data-ttu-id="4f7f4-196">Предоставление `{site-id}` И `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="4f7f4-196">Provide `{site-id}` AND `{item-path}`</span></span> | <span data-ttu-id="4f7f4-197">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-197">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/root:/{item-path}:/children` |
| <span data-ttu-id="4f7f4-198">Предоставление `{user-id}` И `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="4f7f4-198">Provide `{user-id}` AND `{item-path}`</span></span> | <span data-ttu-id="4f7f4-199">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-199">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /users/{user-id}/root:/{item-path}:/children` |
| <span data-ttu-id="4f7f4-200">Предоставление только `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="4f7f4-200">Provide only `{item-path}`</span></span> | <span data-ttu-id="4f7f4-201">Files.Read, Files.Read.All, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-201">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/root:/{item-path}:/children` |
| <span data-ttu-id="4f7f4-202">`insight-type` настроена на трендовую</span><span class="sxs-lookup"><span data-stu-id="4f7f4-202">`insight-type` is set to trending</span></span> | <span data-ttu-id="4f7f4-203">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-203">Sites.Read.All</span></span> | `GET /me/insights/trending` |
| <span data-ttu-id="4f7f4-204">Обеспечить `{user-id or upn}` и `insight-type` установить для `trending`</span><span class="sxs-lookup"><span data-stu-id="4f7f4-204">Provide `{user-id or upn}` AND `insight-type` is set to `trending`</span></span> | <span data-ttu-id="4f7f4-205">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-205">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/trending` | 
| <span data-ttu-id="4f7f4-206">`insight-type` установлено, что `used`</span><span class="sxs-lookup"><span data-stu-id="4f7f4-206">`insight-type` is set to `used`</span></span> | <span data-ttu-id="4f7f4-207">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-207">Sites.Read.All</span></span> | `GET /me/insights/used` |
| <span data-ttu-id="4f7f4-208">Обеспечить `{user-id or upn}` и `insight-type` установить для `used`</span><span class="sxs-lookup"><span data-stu-id="4f7f4-208">Provide `{user-id or upn}` AND `insight-type` is set to `used`</span></span> | <span data-ttu-id="4f7f4-209">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-209">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/used` |
| <span data-ttu-id="4f7f4-210">`insight-type` настроено на общий доступ</span><span class="sxs-lookup"><span data-stu-id="4f7f4-210">`insight-type` is set to shared</span></span> | <span data-ttu-id="4f7f4-211">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-211">Sites.Read.All</span></span> | `GET /me/insights/shared` |
| <span data-ttu-id="4f7f4-212">Обеспечить `{user-id or upn}` и `insight-type` установить для `shared`</span><span class="sxs-lookup"><span data-stu-id="4f7f4-212">Provide `{user-id or upn}` AND `insight-type` is set to `shared`</span></span> | <span data-ttu-id="4f7f4-213">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f4-213">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/shared?$filter=((lastshared/sharedby/id eq '${user-id}') and (resourceReference/type eq 'microsoft.graph.driveItem'))` |

## <a name="events"></a><span data-ttu-id="4f7f4-214">События</span><span class="sxs-lookup"><span data-stu-id="4f7f4-214">Events</span></span>

| <span data-ttu-id="4f7f4-215">Событие</span><span class="sxs-lookup"><span data-stu-id="4f7f4-215">Event</span></span> | <span data-ttu-id="4f7f4-216">Описание</span><span class="sxs-lookup"><span data-stu-id="4f7f4-216">Description</span></span> |
| ----- | ----------- |
| <span data-ttu-id="4f7f4-217">itemClick</span><span class="sxs-lookup"><span data-stu-id="4f7f4-217">itemClick</span></span> | <span data-ttu-id="4f7f4-218">Уволили, когда пользователь щелкнуть файл.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-218">Fired when the user clicks a file.</span></span> <span data-ttu-id="4f7f4-219">Возвращает сведения о файле.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-219">Returns the file details.</span></span> |

## <a name="templates"></a><span data-ttu-id="4f7f4-220">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="4f7f4-220">Templates</span></span>

<span data-ttu-id="4f7f4-221">Компонент `mgt-file-list` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-221">The `mgt-file-list` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="4f7f4-222">Чтобы указать шаблон, включи элемент внутри компонента и закажите значение для одного из типов данных, перечисленных `<template>` `data-type` в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-222">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the data types listed in the following table.</span></span>

| <span data-ttu-id="4f7f4-223">Тип данных</span><span class="sxs-lookup"><span data-stu-id="4f7f4-223">Data type</span></span> | <span data-ttu-id="4f7f4-224">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="4f7f4-224">Data context</span></span> | <span data-ttu-id="4f7f4-225">Описание</span><span class="sxs-lookup"><span data-stu-id="4f7f4-225">Description</span></span> |
| ----------- | -------------- | ------------ |
| <span data-ttu-id="4f7f4-226">default</span><span class="sxs-lookup"><span data-stu-id="4f7f4-226">default</span></span> | <span data-ttu-id="4f7f4-227">`files`: список объектов файлов</span><span class="sxs-lookup"><span data-stu-id="4f7f4-227">`files`: list of file objects</span></span> | <span data-ttu-id="4f7f4-228">Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-228">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="4f7f4-229">file</span><span class="sxs-lookup"><span data-stu-id="4f7f4-229">file</span></span> | <span data-ttu-id="4f7f4-230">`file`: объект файла</span><span class="sxs-lookup"><span data-stu-id="4f7f4-230">`file`: file object</span></span> | <span data-ttu-id="4f7f4-231">Шаблон, используемый для отрисовки каждого файла.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-231">The template used to render each file.</span></span> |
| <span data-ttu-id="4f7f4-232">no-data</span><span class="sxs-lookup"><span data-stu-id="4f7f4-232">no-data</span></span> | <span data-ttu-id="4f7f4-233">Контекст данных не передан</span><span class="sxs-lookup"><span data-stu-id="4f7f4-233">No data context is passed</span></span> | <span data-ttu-id="4f7f4-234">Шаблон, используемый, если данные недоступны.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-234">The template used when no data is available.</span></span> |
| <span data-ttu-id="4f7f4-235">loading</span><span class="sxs-lookup"><span data-stu-id="4f7f4-235">loading</span></span> | <span data-ttu-id="4f7f4-236">Контекст данных не передан</span><span class="sxs-lookup"><span data-stu-id="4f7f4-236">No data context is passed</span></span> | <span data-ttu-id="4f7f4-237">Шаблон, используемый при загрузке состояния компонента.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-237">The template used while the component loads state.</span></span> |

## <a name="authentication"></a><span data-ttu-id="4f7f4-238">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="4f7f4-238">Authentication</span></span>

<span data-ttu-id="4f7f4-239">Для получения требуемых данных в средстве управления используется глобальный поставщик проверки подлинности, указанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="4f7f4-239">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="cache"></a><span data-ttu-id="4f7f4-240">Кэш</span><span class="sxs-lookup"><span data-stu-id="4f7f4-240">Cache</span></span>

|<span data-ttu-id="4f7f4-241">Хранилище объектов</span><span class="sxs-lookup"><span data-stu-id="4f7f4-241">Object store</span></span>|<span data-ttu-id="4f7f4-242">Кэшные данные</span><span class="sxs-lookup"><span data-stu-id="4f7f4-242">Cached data</span></span>|<span data-ttu-id="4f7f4-243">Примечания</span><span class="sxs-lookup"><span data-stu-id="4f7f4-243">Remarks</span></span>|
|---------|-----------|-------|
|`fileLists`|<span data-ttu-id="4f7f4-244">Список списков файлов</span><span class="sxs-lookup"><span data-stu-id="4f7f4-244">List of file lists</span></span>|<span data-ttu-id="4f7f4-245">Список кэша по умолчанию для хранения списков файлов.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-245">Default cache list to store file lists.</span></span>|
|`insightfileLists`|<span data-ttu-id="4f7f4-246">Список списков файлов анализа</span><span class="sxs-lookup"><span data-stu-id="4f7f4-246">List of insight file lists</span></span>|<span data-ttu-id="4f7f4-247">Используется при `insightType` условии.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-247">Used when `insightType` is provided.</span></span>|

> [!NOTE]
> <span data-ttu-id="4f7f4-248">Компонент `mgt-file-list` также использует хранилище объектов в IndexedDB для `fileQueries` `mgt-file` кэша файлов при `fileQueries` условии.</span><span class="sxs-lookup"><span data-stu-id="4f7f4-248">The `mgt-file-list` component also uses the `fileQueries` object store in `mgt-file` IndexedDB to cache files when `fileQueries` is provided.</span></span>

<span data-ttu-id="4f7f4-249">Сведения о настройке кэша см. в материале [Caching.](../customize-components/cache.md)</span><span class="sxs-lookup"><span data-stu-id="4f7f4-249">For details about how to configure the cache, see [Caching](../customize-components/cache.md).</span></span>