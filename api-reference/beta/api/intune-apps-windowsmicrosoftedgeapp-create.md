---
title: Создание Виндовсмикрософтеджеапп
description: Создание нового объекта Виндовсмикрософтеджеапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 41dbf19434aa39f5d8d11b02ec5c5212c36fd248
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444821"
---
# <a name="create-windowsmicrosoftedgeapp"></a><span data-ttu-id="fcb94-103">Создание Виндовсмикрософтеджеапп</span><span class="sxs-lookup"><span data-stu-id="fcb94-103">Create windowsMicrosoftEdgeApp</span></span>

<span data-ttu-id="fcb94-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fcb94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fcb94-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcb94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fcb94-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fcb94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcb94-107">Создание нового объекта [виндовсмикрософтеджеапп](../resources/intune-apps-windowsmicrosoftedgeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="fcb94-107">Create a new [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcb94-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fcb94-108">Prerequisites</span></span>
<span data-ttu-id="fcb94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcb94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcb94-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcb94-111">Permission type</span></span>|<span data-ttu-id="fcb94-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcb94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcb94-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcb94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fcb94-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcb94-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fcb94-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcb94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcb94-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcb94-116">Not supported.</span></span>|
|<span data-ttu-id="fcb94-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcb94-117">Application</span></span>|<span data-ttu-id="fcb94-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcb94-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcb94-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcb94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fcb94-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fcb94-120">Request headers</span></span>
|<span data-ttu-id="fcb94-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcb94-121">Header</span></span>|<span data-ttu-id="fcb94-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fcb94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcb94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcb94-123">Authorization</span></span>|<span data-ttu-id="fcb94-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcb94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcb94-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fcb94-125">Accept</span></span>|<span data-ttu-id="fcb94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fcb94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcb94-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcb94-127">Request body</span></span>
<span data-ttu-id="fcb94-128">В тексте запроса добавьте представление объекта Виндовсмикрософтеджеапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcb94-128">In the request body, supply a JSON representation for the windowsMicrosoftEdgeApp object.</span></span>

<span data-ttu-id="fcb94-129">В следующей таблице приведены свойства, необходимые при создании Виндовсмикрософтеджеапп.</span><span class="sxs-lookup"><span data-stu-id="fcb94-129">The following table shows the properties that are required when you create the windowsMicrosoftEdgeApp.</span></span>

|<span data-ttu-id="fcb94-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcb94-130">Property</span></span>|<span data-ttu-id="fcb94-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fcb94-131">Type</span></span>|<span data-ttu-id="fcb94-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fcb94-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcb94-133">id</span><span class="sxs-lookup"><span data-stu-id="fcb94-133">id</span></span>|<span data-ttu-id="fcb94-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fcb94-134">String</span></span>|<span data-ttu-id="fcb94-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fcb94-135">Key of the entity.</span></span> <span data-ttu-id="fcb94-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fcb94-137">displayName</span></span>|<span data-ttu-id="fcb94-138">Строка</span><span class="sxs-lookup"><span data-stu-id="fcb94-138">String</span></span>|<span data-ttu-id="fcb94-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="fcb94-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fcb94-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-141">description</span><span class="sxs-lookup"><span data-stu-id="fcb94-141">description</span></span>|<span data-ttu-id="fcb94-142">Строка</span><span class="sxs-lookup"><span data-stu-id="fcb94-142">String</span></span>|<span data-ttu-id="fcb94-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="fcb94-143">The description of the app.</span></span> <span data-ttu-id="fcb94-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-145">publisher</span><span class="sxs-lookup"><span data-stu-id="fcb94-145">publisher</span></span>|<span data-ttu-id="fcb94-146">String</span><span class="sxs-lookup"><span data-stu-id="fcb94-146">String</span></span>|<span data-ttu-id="fcb94-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="fcb94-147">The publisher of the app.</span></span> <span data-ttu-id="fcb94-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fcb94-149">largeIcon</span></span>|[<span data-ttu-id="fcb94-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fcb94-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fcb94-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="fcb94-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fcb94-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fcb94-153">createdDateTime</span></span>|<span data-ttu-id="fcb94-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcb94-154">DateTimeOffset</span></span>|<span data-ttu-id="fcb94-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="fcb94-155">The date and time the app was created.</span></span> <span data-ttu-id="fcb94-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fcb94-157">lastModifiedDateTime</span></span>|<span data-ttu-id="fcb94-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcb94-158">DateTimeOffset</span></span>|<span data-ttu-id="fcb94-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="fcb94-159">The date and time the app was last modified.</span></span> <span data-ttu-id="fcb94-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fcb94-161">isFeatured</span></span>|<span data-ttu-id="fcb94-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="fcb94-162">Boolean</span></span>|<span data-ttu-id="fcb94-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fcb94-164">privacyInformationUrl</span></span>|<span data-ttu-id="fcb94-165">String</span><span class="sxs-lookup"><span data-stu-id="fcb94-165">String</span></span>|<span data-ttu-id="fcb94-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="fcb94-166">The privacy statement Url.</span></span> <span data-ttu-id="fcb94-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fcb94-168">informationUrl</span></span>|<span data-ttu-id="fcb94-169">String</span><span class="sxs-lookup"><span data-stu-id="fcb94-169">String</span></span>|<span data-ttu-id="fcb94-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="fcb94-170">The more information Url.</span></span> <span data-ttu-id="fcb94-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-172">owner</span><span class="sxs-lookup"><span data-stu-id="fcb94-172">owner</span></span>|<span data-ttu-id="fcb94-173">String</span><span class="sxs-lookup"><span data-stu-id="fcb94-173">String</span></span>|<span data-ttu-id="fcb94-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="fcb94-174">The owner of the app.</span></span> <span data-ttu-id="fcb94-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-176">developer</span><span class="sxs-lookup"><span data-stu-id="fcb94-176">developer</span></span>|<span data-ttu-id="fcb94-177">String</span><span class="sxs-lookup"><span data-stu-id="fcb94-177">String</span></span>|<span data-ttu-id="fcb94-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="fcb94-178">The developer of the app.</span></span> <span data-ttu-id="fcb94-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-180">notes</span><span class="sxs-lookup"><span data-stu-id="fcb94-180">notes</span></span>|<span data-ttu-id="fcb94-181">String</span><span class="sxs-lookup"><span data-stu-id="fcb94-181">String</span></span>|<span data-ttu-id="fcb94-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="fcb94-182">Notes for the app.</span></span> <span data-ttu-id="fcb94-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="fcb94-184">uploadState</span></span>|<span data-ttu-id="fcb94-185">Int32</span><span class="sxs-lookup"><span data-stu-id="fcb94-185">Int32</span></span>|<span data-ttu-id="fcb94-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="fcb94-186">The upload state.</span></span> <span data-ttu-id="fcb94-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="fcb94-188">publishingState</span></span>|[<span data-ttu-id="fcb94-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="fcb94-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fcb94-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="fcb94-190">The publishing state for the app.</span></span> <span data-ttu-id="fcb94-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="fcb94-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fcb94-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="fcb94-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="fcb94-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fcb94-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fcb94-194">isAssigned</span></span>|<span data-ttu-id="fcb94-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="fcb94-195">Boolean</span></span>|<span data-ttu-id="fcb94-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="fcb94-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="fcb94-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fcb94-198">roleScopeTagIds</span></span>|<span data-ttu-id="fcb94-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fcb94-199">String collection</span></span>|<span data-ttu-id="fcb94-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="fcb94-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="fcb94-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="fcb94-202">dependentAppCount</span></span>|<span data-ttu-id="fcb94-203">Int32</span><span class="sxs-lookup"><span data-stu-id="fcb94-203">Int32</span></span>|<span data-ttu-id="fcb94-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="fcb94-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="fcb94-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fcb94-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fcb94-206">оптоволокон</span><span class="sxs-lookup"><span data-stu-id="fcb94-206">channel</span></span>|[<span data-ttu-id="fcb94-207">microsoftEdgeChannel</span><span class="sxs-lookup"><span data-stu-id="fcb94-207">microsoftEdgeChannel</span></span>](../resources/intune-apps-microsoftedgechannel.md)|<span data-ttu-id="fcb94-208">Канал, который необходимо установить на целевые устройства.</span><span class="sxs-lookup"><span data-stu-id="fcb94-208">The channel to install on target devices.</span></span> <span data-ttu-id="fcb94-209">Возможные значения: `dev`, `beta`, `stable`.</span><span class="sxs-lookup"><span data-stu-id="fcb94-209">Possible values are: `dev`, `beta`, `stable`.</span></span>|
|<span data-ttu-id="fcb94-210">дисплайлангуажелокале</span><span class="sxs-lookup"><span data-stu-id="fcb94-210">displayLanguageLocale</span></span>|<span data-ttu-id="fcb94-211">String</span><span class="sxs-lookup"><span data-stu-id="fcb94-211">String</span></span>|<span data-ttu-id="fcb94-212">Языковой стандарт, используемый при отображении текста для пользователя в пограничной приложении.</span><span class="sxs-lookup"><span data-stu-id="fcb94-212">The language locale to use when the Edge app displays text to the user.</span></span>|



## <a name="response"></a><span data-ttu-id="fcb94-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcb94-213">Response</span></span>
<span data-ttu-id="fcb94-214">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсмикрософтеджеапп](../resources/intune-apps-windowsmicrosoftedgeapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fcb94-214">If successful, this method returns a `201 Created` response code and a [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcb94-215">Пример</span><span class="sxs-lookup"><span data-stu-id="fcb94-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcb94-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcb94-216">Request</span></span>
<span data-ttu-id="fcb94-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcb94-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 805

{
  "@odata.type": "#microsoft.graph.windowsMicrosoftEdgeApp",
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
  "channel": "beta",
  "displayLanguageLocale": "Display Language Locale value"
}
```

### <a name="response"></a><span data-ttu-id="fcb94-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcb94-218">Response</span></span>
<span data-ttu-id="fcb94-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fcb94-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 977

{
  "@odata.type": "#microsoft.graph.windowsMicrosoftEdgeApp",
  "id": "a4d4a316-a316-a4d4-16a3-d4a416a3d4a4",
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
  "channel": "beta",
  "displayLanguageLocale": "Display Language Locale value"
}
```





