---
title: Создание windowsPhone81StoreApp
description: Создание нового объекта WindowsPhone81StoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ac8e0021dd73e34a66e260be1d22fc138da02843
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127020"
---
# <a name="create-windowsphone81storeapp"></a><span data-ttu-id="5cc6f-103">Создание windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="5cc6f-103">Create windowsPhone81StoreApp</span></span>

<span data-ttu-id="5cc6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cc6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5cc6f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cc6f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cc6f-107">Создание нового [объекта WindowsPhone81StoreApp.](../resources/intune-apps-windowsphone81storeapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc6f-107">Create a new [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cc6f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5cc6f-108">Prerequisites</span></span>
<span data-ttu-id="5cc6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cc6f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cc6f-111">Permission type</span></span>|<span data-ttu-id="5cc6f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cc6f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cc6f-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cc6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5cc6f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cc6f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5cc6f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cc6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cc6f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-116">Not supported.</span></span>|
|<span data-ttu-id="5cc6f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5cc6f-117">Application</span></span>|<span data-ttu-id="5cc6f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cc6f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cc6f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cc6f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5cc6f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5cc6f-120">Request headers</span></span>
|<span data-ttu-id="5cc6f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5cc6f-121">Header</span></span>|<span data-ttu-id="5cc6f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5cc6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cc6f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cc6f-123">Authorization</span></span>|<span data-ttu-id="5cc6f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cc6f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5cc6f-125">Accept</span></span>|<span data-ttu-id="5cc6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5cc6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cc6f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5cc6f-127">Request body</span></span>
<span data-ttu-id="5cc6f-128">В корпусе запроса поставляем представление JSON для объекта WindowsPhone81StoreApp.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-128">In the request body, supply a JSON representation for the windowsPhone81StoreApp object.</span></span>

<span data-ttu-id="5cc6f-129">В следующей таблице показаны свойства, необходимые при создании windowsPhone81StoreApp.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-129">The following table shows the properties that are required when you create the windowsPhone81StoreApp.</span></span>

|<span data-ttu-id="5cc6f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cc6f-130">Property</span></span>|<span data-ttu-id="5cc6f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5cc6f-131">Type</span></span>|<span data-ttu-id="5cc6f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5cc6f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cc6f-133">id</span><span class="sxs-lookup"><span data-stu-id="5cc6f-133">id</span></span>|<span data-ttu-id="5cc6f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5cc6f-134">String</span></span>|<span data-ttu-id="5cc6f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-135">Key of the entity.</span></span> <span data-ttu-id="5cc6f-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5cc6f-137">displayName</span></span>|<span data-ttu-id="5cc6f-138">Строка</span><span class="sxs-lookup"><span data-stu-id="5cc6f-138">String</span></span>|<span data-ttu-id="5cc6f-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5cc6f-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-141">description</span><span class="sxs-lookup"><span data-stu-id="5cc6f-141">description</span></span>|<span data-ttu-id="5cc6f-142">Строка</span><span class="sxs-lookup"><span data-stu-id="5cc6f-142">String</span></span>|<span data-ttu-id="5cc6f-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-143">The description of the app.</span></span> <span data-ttu-id="5cc6f-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-145">publisher</span><span class="sxs-lookup"><span data-stu-id="5cc6f-145">publisher</span></span>|<span data-ttu-id="5cc6f-146">String</span><span class="sxs-lookup"><span data-stu-id="5cc6f-146">String</span></span>|<span data-ttu-id="5cc6f-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-147">The publisher of the app.</span></span> <span data-ttu-id="5cc6f-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5cc6f-149">largeIcon</span></span>|[<span data-ttu-id="5cc6f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5cc6f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5cc6f-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5cc6f-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5cc6f-153">createdDateTime</span></span>|<span data-ttu-id="5cc6f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cc6f-154">DateTimeOffset</span></span>|<span data-ttu-id="5cc6f-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-155">The date and time the app was created.</span></span> <span data-ttu-id="5cc6f-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cc6f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="5cc6f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cc6f-158">DateTimeOffset</span></span>|<span data-ttu-id="5cc6f-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="5cc6f-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5cc6f-161">isFeatured</span></span>|<span data-ttu-id="5cc6f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="5cc6f-162">Boolean</span></span>|<span data-ttu-id="5cc6f-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5cc6f-164">privacyInformationUrl</span></span>|<span data-ttu-id="5cc6f-165">String</span><span class="sxs-lookup"><span data-stu-id="5cc6f-165">String</span></span>|<span data-ttu-id="5cc6f-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-166">The privacy statement Url.</span></span> <span data-ttu-id="5cc6f-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5cc6f-168">informationUrl</span></span>|<span data-ttu-id="5cc6f-169">String</span><span class="sxs-lookup"><span data-stu-id="5cc6f-169">String</span></span>|<span data-ttu-id="5cc6f-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-170">The more information Url.</span></span> <span data-ttu-id="5cc6f-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-172">owner</span><span class="sxs-lookup"><span data-stu-id="5cc6f-172">owner</span></span>|<span data-ttu-id="5cc6f-173">String</span><span class="sxs-lookup"><span data-stu-id="5cc6f-173">String</span></span>|<span data-ttu-id="5cc6f-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-174">The owner of the app.</span></span> <span data-ttu-id="5cc6f-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-176">developer</span><span class="sxs-lookup"><span data-stu-id="5cc6f-176">developer</span></span>|<span data-ttu-id="5cc6f-177">String</span><span class="sxs-lookup"><span data-stu-id="5cc6f-177">String</span></span>|<span data-ttu-id="5cc6f-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-178">The developer of the app.</span></span> <span data-ttu-id="5cc6f-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-180">notes</span><span class="sxs-lookup"><span data-stu-id="5cc6f-180">notes</span></span>|<span data-ttu-id="5cc6f-181">String</span><span class="sxs-lookup"><span data-stu-id="5cc6f-181">String</span></span>|<span data-ttu-id="5cc6f-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-182">Notes for the app.</span></span> <span data-ttu-id="5cc6f-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="5cc6f-184">uploadState</span></span>|<span data-ttu-id="5cc6f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="5cc6f-185">Int32</span></span>|<span data-ttu-id="5cc6f-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-186">The upload state.</span></span> <span data-ttu-id="5cc6f-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="5cc6f-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="5cc6f-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="5cc6f-189">publishingState</span></span>|[<span data-ttu-id="5cc6f-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5cc6f-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5cc6f-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-191">The publishing state for the app.</span></span> <span data-ttu-id="5cc6f-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5cc6f-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="5cc6f-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5cc6f-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5cc6f-195">isAssigned</span></span>|<span data-ttu-id="5cc6f-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="5cc6f-196">Boolean</span></span>|<span data-ttu-id="5cc6f-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="5cc6f-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5cc6f-199">roleScopeTagIds</span></span>|<span data-ttu-id="5cc6f-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5cc6f-200">String collection</span></span>|<span data-ttu-id="5cc6f-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="5cc6f-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="5cc6f-203">dependentAppCount</span></span>|<span data-ttu-id="5cc6f-204">Int32</span><span class="sxs-lookup"><span data-stu-id="5cc6f-204">Int32</span></span>|<span data-ttu-id="5cc6f-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="5cc6f-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="5cc6f-207">supersedingAppCount</span></span>|<span data-ttu-id="5cc6f-208">Int32</span><span class="sxs-lookup"><span data-stu-id="5cc6f-208">Int32</span></span>|<span data-ttu-id="5cc6f-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="5cc6f-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="5cc6f-211">supersededAppCount</span></span>|<span data-ttu-id="5cc6f-212">Int32</span><span class="sxs-lookup"><span data-stu-id="5cc6f-212">Int32</span></span>|<span data-ttu-id="5cc6f-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="5cc6f-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cc6f-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc6f-215">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="5cc6f-215">appStoreUrl</span></span>|<span data-ttu-id="5cc6f-216">String</span><span class="sxs-lookup"><span data-stu-id="5cc6f-216">String</span></span>|<span data-ttu-id="5cc6f-217">URL-адрес магазина приложений Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-217">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="5cc6f-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cc6f-218">Response</span></span>
<span data-ttu-id="5cc6f-219">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект WindowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-219">If successful, this method returns a `201 Created` response code and a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cc6f-220">Пример</span><span class="sxs-lookup"><span data-stu-id="5cc6f-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cc6f-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cc6f-221">Request</span></span>
<span data-ttu-id="5cc6f-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 832

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="5cc6f-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cc6f-223">Response</span></span>
<span data-ttu-id="5cc6f-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5cc6f-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1004

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
  "id": "f68ce6a1-e6a1-f68c-a1e6-8cf6a1e68cf6",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




