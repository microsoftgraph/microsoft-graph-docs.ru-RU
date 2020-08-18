---
title: Обновление Макосмикрософтеджеапп
description: Обновление свойств объекта Макосмикрософтеджеапп.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 779a8cf934b0becddaa97f9c53e8168072e3befc
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792046"
---
# <a name="update-macosmicrosoftedgeapp"></a><span data-ttu-id="527fc-103">Обновление Макосмикрософтеджеапп</span><span class="sxs-lookup"><span data-stu-id="527fc-103">Update macOSMicrosoftEdgeApp</span></span>

<span data-ttu-id="527fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="527fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="527fc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="527fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="527fc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="527fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="527fc-107">Обновление свойств объекта [макосмикрософтеджеапп](../resources/intune-apps-macosmicrosoftedgeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="527fc-107">Update the properties of a [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="527fc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="527fc-108">Prerequisites</span></span>
<span data-ttu-id="527fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="527fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="527fc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="527fc-111">Permission type</span></span>|<span data-ttu-id="527fc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="527fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="527fc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="527fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="527fc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="527fc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="527fc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="527fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="527fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="527fc-116">Not supported.</span></span>|
|<span data-ttu-id="527fc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="527fc-117">Application</span></span>|<span data-ttu-id="527fc-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="527fc-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="527fc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="527fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="527fc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="527fc-120">Request headers</span></span>
|<span data-ttu-id="527fc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="527fc-121">Header</span></span>|<span data-ttu-id="527fc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="527fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="527fc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="527fc-123">Authorization</span></span>|<span data-ttu-id="527fc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="527fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="527fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="527fc-125">Accept</span></span>|<span data-ttu-id="527fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="527fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="527fc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="527fc-127">Request body</span></span>
<span data-ttu-id="527fc-128">В тексте запроса добавьте представление объекта [макосмикрософтеджеапп](../resources/intune-apps-macosmicrosoftedgeapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="527fc-128">In the request body, supply a JSON representation for the [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object.</span></span>

<span data-ttu-id="527fc-129">В следующей таблице приведены свойства, необходимые при создании [макосмикрософтеджеапп](../resources/intune-apps-macosmicrosoftedgeapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-129">The following table shows the properties that are required when you create the [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md).</span></span>

|<span data-ttu-id="527fc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="527fc-130">Property</span></span>|<span data-ttu-id="527fc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="527fc-131">Type</span></span>|<span data-ttu-id="527fc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="527fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="527fc-133">id</span><span class="sxs-lookup"><span data-stu-id="527fc-133">id</span></span>|<span data-ttu-id="527fc-134">String</span><span class="sxs-lookup"><span data-stu-id="527fc-134">String</span></span>|<span data-ttu-id="527fc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="527fc-135">Key of the entity.</span></span> <span data-ttu-id="527fc-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="527fc-137">displayName</span></span>|<span data-ttu-id="527fc-138">String</span><span class="sxs-lookup"><span data-stu-id="527fc-138">String</span></span>|<span data-ttu-id="527fc-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="527fc-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="527fc-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-141">description</span><span class="sxs-lookup"><span data-stu-id="527fc-141">description</span></span>|<span data-ttu-id="527fc-142">String</span><span class="sxs-lookup"><span data-stu-id="527fc-142">String</span></span>|<span data-ttu-id="527fc-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="527fc-143">The description of the app.</span></span> <span data-ttu-id="527fc-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-145">publisher</span><span class="sxs-lookup"><span data-stu-id="527fc-145">publisher</span></span>|<span data-ttu-id="527fc-146">String</span><span class="sxs-lookup"><span data-stu-id="527fc-146">String</span></span>|<span data-ttu-id="527fc-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="527fc-147">The publisher of the app.</span></span> <span data-ttu-id="527fc-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="527fc-149">largeIcon</span></span>|[<span data-ttu-id="527fc-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="527fc-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="527fc-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="527fc-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="527fc-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="527fc-153">createdDateTime</span></span>|<span data-ttu-id="527fc-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="527fc-154">DateTimeOffset</span></span>|<span data-ttu-id="527fc-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="527fc-155">The date and time the app was created.</span></span> <span data-ttu-id="527fc-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="527fc-157">lastModifiedDateTime</span></span>|<span data-ttu-id="527fc-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="527fc-158">DateTimeOffset</span></span>|<span data-ttu-id="527fc-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="527fc-159">The date and time the app was last modified.</span></span> <span data-ttu-id="527fc-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="527fc-161">isFeatured</span></span>|<span data-ttu-id="527fc-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="527fc-162">Boolean</span></span>|<span data-ttu-id="527fc-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="527fc-164">privacyInformationUrl</span></span>|<span data-ttu-id="527fc-165">String</span><span class="sxs-lookup"><span data-stu-id="527fc-165">String</span></span>|<span data-ttu-id="527fc-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="527fc-166">The privacy statement Url.</span></span> <span data-ttu-id="527fc-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="527fc-168">informationUrl</span></span>|<span data-ttu-id="527fc-169">String</span><span class="sxs-lookup"><span data-stu-id="527fc-169">String</span></span>|<span data-ttu-id="527fc-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="527fc-170">The more information Url.</span></span> <span data-ttu-id="527fc-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-172">owner</span><span class="sxs-lookup"><span data-stu-id="527fc-172">owner</span></span>|<span data-ttu-id="527fc-173">String</span><span class="sxs-lookup"><span data-stu-id="527fc-173">String</span></span>|<span data-ttu-id="527fc-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="527fc-174">The owner of the app.</span></span> <span data-ttu-id="527fc-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-176">developer</span><span class="sxs-lookup"><span data-stu-id="527fc-176">developer</span></span>|<span data-ttu-id="527fc-177">String</span><span class="sxs-lookup"><span data-stu-id="527fc-177">String</span></span>|<span data-ttu-id="527fc-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="527fc-178">The developer of the app.</span></span> <span data-ttu-id="527fc-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-180">notes</span><span class="sxs-lookup"><span data-stu-id="527fc-180">notes</span></span>|<span data-ttu-id="527fc-181">String</span><span class="sxs-lookup"><span data-stu-id="527fc-181">String</span></span>|<span data-ttu-id="527fc-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="527fc-182">Notes for the app.</span></span> <span data-ttu-id="527fc-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="527fc-184">uploadState</span></span>|<span data-ttu-id="527fc-185">Int32</span><span class="sxs-lookup"><span data-stu-id="527fc-185">Int32</span></span>|<span data-ttu-id="527fc-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="527fc-186">The upload state.</span></span> <span data-ttu-id="527fc-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="527fc-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="527fc-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="527fc-189">publishingState</span></span>|[<span data-ttu-id="527fc-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="527fc-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="527fc-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="527fc-191">The publishing state for the app.</span></span> <span data-ttu-id="527fc-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="527fc-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="527fc-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="527fc-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="527fc-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="527fc-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="527fc-195">isAssigned</span></span>|<span data-ttu-id="527fc-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="527fc-196">Boolean</span></span>|<span data-ttu-id="527fc-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="527fc-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="527fc-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="527fc-199">roleScopeTagIds</span></span>|<span data-ttu-id="527fc-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="527fc-200">String collection</span></span>|<span data-ttu-id="527fc-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="527fc-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="527fc-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="527fc-203">dependentAppCount</span></span>|<span data-ttu-id="527fc-204">Int32</span><span class="sxs-lookup"><span data-stu-id="527fc-204">Int32</span></span>|<span data-ttu-id="527fc-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="527fc-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="527fc-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="527fc-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="527fc-207">channel</span><span class="sxs-lookup"><span data-stu-id="527fc-207">channel</span></span>|[<span data-ttu-id="527fc-208">microsoftEdgeChannel</span><span class="sxs-lookup"><span data-stu-id="527fc-208">microsoftEdgeChannel</span></span>](../resources/intune-apps-microsoftedgechannel.md)|<span data-ttu-id="527fc-209">Канал, который необходимо установить на целевые устройства.</span><span class="sxs-lookup"><span data-stu-id="527fc-209">The channel to install on target devices.</span></span> <span data-ttu-id="527fc-210">Возможные значения: `dev`, `beta`, `stable`.</span><span class="sxs-lookup"><span data-stu-id="527fc-210">Possible values are: `dev`, `beta`, `stable`.</span></span>|



## <a name="response"></a><span data-ttu-id="527fc-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="527fc-211">Response</span></span>
<span data-ttu-id="527fc-212">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосмикрософтеджеапп](../resources/intune-apps-macosmicrosoftedgeapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="527fc-212">If successful, this method returns a `200 OK` response code and an updated [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="527fc-213">Пример</span><span class="sxs-lookup"><span data-stu-id="527fc-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="527fc-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="527fc-214">Request</span></span>
<span data-ttu-id="527fc-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="527fc-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 742

{
  "@odata.type": "#microsoft.graph.macOSMicrosoftEdgeApp",
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
  "channel": "beta"
}
```

### <a name="response"></a><span data-ttu-id="527fc-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="527fc-216">Response</span></span>
<span data-ttu-id="527fc-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="527fc-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

{
  "@odata.type": "#microsoft.graph.macOSMicrosoftEdgeApp",
  "id": "c964092a-092a-c964-2a09-64c92a0964c9",
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
  "channel": "beta"
}
```



