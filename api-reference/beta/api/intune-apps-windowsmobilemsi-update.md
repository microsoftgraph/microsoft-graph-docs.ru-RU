---
title: Update windowsMobileMSI
description: Обновление свойств объекта windowsMobileMSI.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 500d20789977f1a76ca255c4d7d6d3e2d5fad684
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791017"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="222d1-103">Update windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="222d1-103">Update windowsMobileMSI</span></span>

<span data-ttu-id="222d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="222d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="222d1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="222d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="222d1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="222d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="222d1-107">Обновление свойств объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-107">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="222d1-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="222d1-108">Prerequisites</span></span>
<span data-ttu-id="222d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="222d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="222d1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="222d1-111">Permission type</span></span>|<span data-ttu-id="222d1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="222d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="222d1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="222d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="222d1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="222d1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="222d1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="222d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="222d1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="222d1-116">Not supported.</span></span>|
|<span data-ttu-id="222d1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="222d1-117">Application</span></span>|<span data-ttu-id="222d1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="222d1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="222d1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="222d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="222d1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="222d1-120">Request headers</span></span>
|<span data-ttu-id="222d1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="222d1-121">Header</span></span>|<span data-ttu-id="222d1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="222d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="222d1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="222d1-123">Authorization</span></span>|<span data-ttu-id="222d1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="222d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="222d1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="222d1-125">Accept</span></span>|<span data-ttu-id="222d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="222d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="222d1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="222d1-127">Request body</span></span>
<span data-ttu-id="222d1-128">В теле запроса добавьте представление объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="222d1-128">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="222d1-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-129">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="222d1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="222d1-130">Property</span></span>|<span data-ttu-id="222d1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="222d1-131">Type</span></span>|<span data-ttu-id="222d1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="222d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="222d1-133">id</span><span class="sxs-lookup"><span data-stu-id="222d1-133">id</span></span>|<span data-ttu-id="222d1-134">String</span><span class="sxs-lookup"><span data-stu-id="222d1-134">String</span></span>|<span data-ttu-id="222d1-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="222d1-135">Key of the entity.</span></span> <span data-ttu-id="222d1-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-137">displayName</span><span class="sxs-lookup"><span data-stu-id="222d1-137">displayName</span></span>|<span data-ttu-id="222d1-138">String</span><span class="sxs-lookup"><span data-stu-id="222d1-138">String</span></span>|<span data-ttu-id="222d1-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="222d1-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="222d1-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-141">description</span><span class="sxs-lookup"><span data-stu-id="222d1-141">description</span></span>|<span data-ttu-id="222d1-142">String</span><span class="sxs-lookup"><span data-stu-id="222d1-142">String</span></span>|<span data-ttu-id="222d1-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="222d1-143">The description of the app.</span></span> <span data-ttu-id="222d1-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-145">publisher</span><span class="sxs-lookup"><span data-stu-id="222d1-145">publisher</span></span>|<span data-ttu-id="222d1-146">String</span><span class="sxs-lookup"><span data-stu-id="222d1-146">String</span></span>|<span data-ttu-id="222d1-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="222d1-147">The publisher of the app.</span></span> <span data-ttu-id="222d1-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="222d1-149">largeIcon</span></span>|[<span data-ttu-id="222d1-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="222d1-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="222d1-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="222d1-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="222d1-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="222d1-153">createdDateTime</span></span>|<span data-ttu-id="222d1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="222d1-154">DateTimeOffset</span></span>|<span data-ttu-id="222d1-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="222d1-155">The date and time the app was created.</span></span> <span data-ttu-id="222d1-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="222d1-157">lastModifiedDateTime</span></span>|<span data-ttu-id="222d1-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="222d1-158">DateTimeOffset</span></span>|<span data-ttu-id="222d1-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="222d1-159">The date and time the app was last modified.</span></span> <span data-ttu-id="222d1-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="222d1-161">isFeatured</span></span>|<span data-ttu-id="222d1-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="222d1-162">Boolean</span></span>|<span data-ttu-id="222d1-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="222d1-164">privacyInformationUrl</span></span>|<span data-ttu-id="222d1-165">String</span><span class="sxs-lookup"><span data-stu-id="222d1-165">String</span></span>|<span data-ttu-id="222d1-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="222d1-166">The privacy statement Url.</span></span> <span data-ttu-id="222d1-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="222d1-168">informationUrl</span></span>|<span data-ttu-id="222d1-169">String</span><span class="sxs-lookup"><span data-stu-id="222d1-169">String</span></span>|<span data-ttu-id="222d1-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="222d1-170">The more information Url.</span></span> <span data-ttu-id="222d1-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-172">owner</span><span class="sxs-lookup"><span data-stu-id="222d1-172">owner</span></span>|<span data-ttu-id="222d1-173">String</span><span class="sxs-lookup"><span data-stu-id="222d1-173">String</span></span>|<span data-ttu-id="222d1-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="222d1-174">The owner of the app.</span></span> <span data-ttu-id="222d1-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-176">developer</span><span class="sxs-lookup"><span data-stu-id="222d1-176">developer</span></span>|<span data-ttu-id="222d1-177">String</span><span class="sxs-lookup"><span data-stu-id="222d1-177">String</span></span>|<span data-ttu-id="222d1-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="222d1-178">The developer of the app.</span></span> <span data-ttu-id="222d1-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-180">notes</span><span class="sxs-lookup"><span data-stu-id="222d1-180">notes</span></span>|<span data-ttu-id="222d1-181">String</span><span class="sxs-lookup"><span data-stu-id="222d1-181">String</span></span>|<span data-ttu-id="222d1-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="222d1-182">Notes for the app.</span></span> <span data-ttu-id="222d1-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="222d1-184">uploadState</span></span>|<span data-ttu-id="222d1-185">Int32</span><span class="sxs-lookup"><span data-stu-id="222d1-185">Int32</span></span>|<span data-ttu-id="222d1-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="222d1-186">The upload state.</span></span> <span data-ttu-id="222d1-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="222d1-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="222d1-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="222d1-189">publishingState</span></span>|[<span data-ttu-id="222d1-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="222d1-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="222d1-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="222d1-191">The publishing state for the app.</span></span> <span data-ttu-id="222d1-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="222d1-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="222d1-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="222d1-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="222d1-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="222d1-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="222d1-195">isAssigned</span></span>|<span data-ttu-id="222d1-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="222d1-196">Boolean</span></span>|<span data-ttu-id="222d1-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="222d1-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="222d1-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="222d1-199">roleScopeTagIds</span></span>|<span data-ttu-id="222d1-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="222d1-200">String collection</span></span>|<span data-ttu-id="222d1-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="222d1-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="222d1-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="222d1-203">dependentAppCount</span></span>|<span data-ttu-id="222d1-204">Int32</span><span class="sxs-lookup"><span data-stu-id="222d1-204">Int32</span></span>|<span data-ttu-id="222d1-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="222d1-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="222d1-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="222d1-207">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="222d1-207">committedContentVersion</span></span>|<span data-ttu-id="222d1-208">String</span><span class="sxs-lookup"><span data-stu-id="222d1-208">String</span></span>|<span data-ttu-id="222d1-209">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="222d1-209">The internal committed content version.</span></span> <span data-ttu-id="222d1-210">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-210">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="222d1-211">fileName</span><span class="sxs-lookup"><span data-stu-id="222d1-211">fileName</span></span>|<span data-ttu-id="222d1-212">String</span><span class="sxs-lookup"><span data-stu-id="222d1-212">String</span></span>|<span data-ttu-id="222d1-213">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="222d1-213">The name of the main Lob application file.</span></span> <span data-ttu-id="222d1-214">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-214">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="222d1-215">size</span><span class="sxs-lookup"><span data-stu-id="222d1-215">size</span></span>|<span data-ttu-id="222d1-216">Int64</span><span class="sxs-lookup"><span data-stu-id="222d1-216">Int64</span></span>|<span data-ttu-id="222d1-217">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="222d1-217">The total size, including all uploaded files.</span></span> <span data-ttu-id="222d1-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="222d1-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="222d1-219">commandLine</span><span class="sxs-lookup"><span data-stu-id="222d1-219">commandLine</span></span>|<span data-ttu-id="222d1-220">String</span><span class="sxs-lookup"><span data-stu-id="222d1-220">String</span></span>|<span data-ttu-id="222d1-221">Командная строка.</span><span class="sxs-lookup"><span data-stu-id="222d1-221">The command line.</span></span>|
|<span data-ttu-id="222d1-222">productCode</span><span class="sxs-lookup"><span data-stu-id="222d1-222">productCode</span></span>|<span data-ttu-id="222d1-223">String</span><span class="sxs-lookup"><span data-stu-id="222d1-223">String</span></span>|<span data-ttu-id="222d1-224">Код продукта.</span><span class="sxs-lookup"><span data-stu-id="222d1-224">The product code.</span></span>|
|<span data-ttu-id="222d1-225">productVersion</span><span class="sxs-lookup"><span data-stu-id="222d1-225">productVersion</span></span>|<span data-ttu-id="222d1-226">String</span><span class="sxs-lookup"><span data-stu-id="222d1-226">String</span></span>|<span data-ttu-id="222d1-227">Версия бизнес-приложения, к которому применяется MSI Windows Mobile.</span><span class="sxs-lookup"><span data-stu-id="222d1-227">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="222d1-228">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="222d1-228">ignoreVersionDetection</span></span>|<span data-ttu-id="222d1-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="222d1-229">Boolean</span></span>|<span data-ttu-id="222d1-230">Логическое значение, позволяющее разрешить или запретить поиск установленного приложения по его версии.</span><span class="sxs-lookup"><span data-stu-id="222d1-230">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="222d1-231">Задайте значение true для бизнес-приложений MSI для Windows Mobile с функцией самостоятельного обновления.</span><span class="sxs-lookup"><span data-stu-id="222d1-231">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="222d1-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="222d1-232">identityVersion</span></span>|<span data-ttu-id="222d1-233">String</span><span class="sxs-lookup"><span data-stu-id="222d1-233">String</span></span>|<span data-ttu-id="222d1-234">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="222d1-234">The identity version.</span></span>|
|<span data-ttu-id="222d1-235">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="222d1-235">useDeviceContext</span></span>|<span data-ttu-id="222d1-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="222d1-236">Boolean</span></span>|<span data-ttu-id="222d1-237">Указывает, следует ли установить MSI с двойным режимом в контексте устройства.</span><span class="sxs-lookup"><span data-stu-id="222d1-237">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="222d1-238">Если задано значение true, приложение будет установлено для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="222d1-238">If true, app will be installed for all users.</span></span> <span data-ttu-id="222d1-239">Если задано значение false, приложение будет установлено для каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="222d1-239">If false, app will be installed per-user.</span></span> <span data-ttu-id="222d1-240">Если значение равно null, служба будет использовать стандартный контекст установки пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="222d1-240">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="222d1-241">В случае с двойным режимом MSI это значение по умолчанию будет иметь значение "на пользователя".</span><span class="sxs-lookup"><span data-stu-id="222d1-241">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="222d1-242">Не может быть задано для приложений с несдвоенным режимом.</span><span class="sxs-lookup"><span data-stu-id="222d1-242">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="222d1-243">После первоначального создания приложения его невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="222d1-243">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="222d1-244">Ответ</span><span class="sxs-lookup"><span data-stu-id="222d1-244">Response</span></span>
<span data-ttu-id="222d1-245">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="222d1-245">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="222d1-246">Пример</span><span class="sxs-lookup"><span data-stu-id="222d1-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="222d1-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="222d1-247">Request</span></span>
<span data-ttu-id="222d1-248">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="222d1-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1066

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="222d1-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="222d1-249">Response</span></span>
<span data-ttu-id="222d1-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="222d1-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1238

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```



