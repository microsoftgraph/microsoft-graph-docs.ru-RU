---
title: Create windowsMobileMSI
description: Создание объекта windowsMobileMSI.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f2092d6b227144ec7c6a6df27d6f8f28c27c2b8a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43403716"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="7b07e-103">Create windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="7b07e-103">Create windowsMobileMSI</span></span>

<span data-ttu-id="7b07e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b07e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b07e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b07e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b07e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b07e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b07e-107">Создание объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-107">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b07e-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7b07e-108">Prerequisites</span></span>
<span data-ttu-id="7b07e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b07e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b07e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b07e-111">Permission type</span></span>|<span data-ttu-id="7b07e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b07e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b07e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b07e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b07e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b07e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7b07e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b07e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b07e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b07e-116">Not supported.</span></span>|
|<span data-ttu-id="7b07e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b07e-117">Application</span></span>|<span data-ttu-id="7b07e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b07e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b07e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b07e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7b07e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7b07e-120">Request headers</span></span>
|<span data-ttu-id="7b07e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b07e-121">Header</span></span>|<span data-ttu-id="7b07e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7b07e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b07e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b07e-123">Authorization</span></span>|<span data-ttu-id="7b07e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b07e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b07e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7b07e-125">Accept</span></span>|<span data-ttu-id="7b07e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b07e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b07e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b07e-127">Request body</span></span>
<span data-ttu-id="7b07e-128">В тексте запроса добавьте представление объекта windowsMobileMSI в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b07e-128">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="7b07e-129">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="7b07e-129">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="7b07e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b07e-130">Property</span></span>|<span data-ttu-id="7b07e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7b07e-131">Type</span></span>|<span data-ttu-id="7b07e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7b07e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b07e-133">id</span><span class="sxs-lookup"><span data-stu-id="7b07e-133">id</span></span>|<span data-ttu-id="7b07e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7b07e-134">String</span></span>|<span data-ttu-id="7b07e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7b07e-135">Key of the entity.</span></span> <span data-ttu-id="7b07e-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7b07e-137">displayName</span></span>|<span data-ttu-id="7b07e-138">Строка</span><span class="sxs-lookup"><span data-stu-id="7b07e-138">String</span></span>|<span data-ttu-id="7b07e-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="7b07e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7b07e-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-141">description</span><span class="sxs-lookup"><span data-stu-id="7b07e-141">description</span></span>|<span data-ttu-id="7b07e-142">Строка</span><span class="sxs-lookup"><span data-stu-id="7b07e-142">String</span></span>|<span data-ttu-id="7b07e-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="7b07e-143">The description of the app.</span></span> <span data-ttu-id="7b07e-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="7b07e-145">publisher</span></span>|<span data-ttu-id="7b07e-146">String</span><span class="sxs-lookup"><span data-stu-id="7b07e-146">String</span></span>|<span data-ttu-id="7b07e-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="7b07e-147">The publisher of the app.</span></span> <span data-ttu-id="7b07e-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7b07e-149">largeIcon</span></span>|[<span data-ttu-id="7b07e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7b07e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7b07e-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="7b07e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7b07e-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b07e-153">createdDateTime</span></span>|<span data-ttu-id="7b07e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b07e-154">DateTimeOffset</span></span>|<span data-ttu-id="7b07e-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="7b07e-155">The date and time the app was created.</span></span> <span data-ttu-id="7b07e-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b07e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="7b07e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b07e-158">DateTimeOffset</span></span>|<span data-ttu-id="7b07e-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="7b07e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="7b07e-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7b07e-161">isFeatured</span></span>|<span data-ttu-id="7b07e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b07e-162">Boolean</span></span>|<span data-ttu-id="7b07e-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7b07e-164">privacyInformationUrl</span></span>|<span data-ttu-id="7b07e-165">String</span><span class="sxs-lookup"><span data-stu-id="7b07e-165">String</span></span>|<span data-ttu-id="7b07e-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="7b07e-166">The privacy statement Url.</span></span> <span data-ttu-id="7b07e-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7b07e-168">informationUrl</span></span>|<span data-ttu-id="7b07e-169">String</span><span class="sxs-lookup"><span data-stu-id="7b07e-169">String</span></span>|<span data-ttu-id="7b07e-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="7b07e-170">The more information Url.</span></span> <span data-ttu-id="7b07e-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-172">owner</span><span class="sxs-lookup"><span data-stu-id="7b07e-172">owner</span></span>|<span data-ttu-id="7b07e-173">String</span><span class="sxs-lookup"><span data-stu-id="7b07e-173">String</span></span>|<span data-ttu-id="7b07e-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="7b07e-174">The owner of the app.</span></span> <span data-ttu-id="7b07e-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-176">developer</span><span class="sxs-lookup"><span data-stu-id="7b07e-176">developer</span></span>|<span data-ttu-id="7b07e-177">String</span><span class="sxs-lookup"><span data-stu-id="7b07e-177">String</span></span>|<span data-ttu-id="7b07e-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="7b07e-178">The developer of the app.</span></span> <span data-ttu-id="7b07e-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-180">notes</span><span class="sxs-lookup"><span data-stu-id="7b07e-180">notes</span></span>|<span data-ttu-id="7b07e-181">String</span><span class="sxs-lookup"><span data-stu-id="7b07e-181">String</span></span>|<span data-ttu-id="7b07e-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="7b07e-182">Notes for the app.</span></span> <span data-ttu-id="7b07e-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="7b07e-184">uploadState</span></span>|<span data-ttu-id="7b07e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="7b07e-185">Int32</span></span>|<span data-ttu-id="7b07e-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="7b07e-186">The upload state.</span></span> <span data-ttu-id="7b07e-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="7b07e-188">publishingState</span></span>|[<span data-ttu-id="7b07e-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="7b07e-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7b07e-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="7b07e-190">The publishing state for the app.</span></span> <span data-ttu-id="7b07e-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="7b07e-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7b07e-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="7b07e-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7b07e-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7b07e-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7b07e-194">isAssigned</span></span>|<span data-ttu-id="7b07e-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b07e-195">Boolean</span></span>|<span data-ttu-id="7b07e-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="7b07e-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7b07e-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7b07e-198">roleScopeTagIds</span></span>|<span data-ttu-id="7b07e-199">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="7b07e-199">String collection</span></span>|<span data-ttu-id="7b07e-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="7b07e-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7b07e-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="7b07e-202">dependentAppCount</span></span>|<span data-ttu-id="7b07e-203">Int32</span><span class="sxs-lookup"><span data-stu-id="7b07e-203">Int32</span></span>|<span data-ttu-id="7b07e-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="7b07e-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="7b07e-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7b07e-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="7b07e-206">committedContentVersion</span></span>|<span data-ttu-id="7b07e-207">String</span><span class="sxs-lookup"><span data-stu-id="7b07e-207">String</span></span>|<span data-ttu-id="7b07e-208">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="7b07e-208">The internal committed content version.</span></span> <span data-ttu-id="7b07e-209">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7b07e-210">fileName</span><span class="sxs-lookup"><span data-stu-id="7b07e-210">fileName</span></span>|<span data-ttu-id="7b07e-211">String</span><span class="sxs-lookup"><span data-stu-id="7b07e-211">String</span></span>|<span data-ttu-id="7b07e-212">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="7b07e-212">The name of the main Lob application file.</span></span> <span data-ttu-id="7b07e-213">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7b07e-214">size</span><span class="sxs-lookup"><span data-stu-id="7b07e-214">size</span></span>|<span data-ttu-id="7b07e-215">Int64</span><span class="sxs-lookup"><span data-stu-id="7b07e-215">Int64</span></span>|<span data-ttu-id="7b07e-216">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="7b07e-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="7b07e-217">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b07e-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7b07e-218">commandLine</span><span class="sxs-lookup"><span data-stu-id="7b07e-218">commandLine</span></span>|<span data-ttu-id="7b07e-219">String</span><span class="sxs-lookup"><span data-stu-id="7b07e-219">String</span></span>|<span data-ttu-id="7b07e-220">Командная строка.</span><span class="sxs-lookup"><span data-stu-id="7b07e-220">The command line.</span></span>|
|<span data-ttu-id="7b07e-221">productCode</span><span class="sxs-lookup"><span data-stu-id="7b07e-221">productCode</span></span>|<span data-ttu-id="7b07e-222">String</span><span class="sxs-lookup"><span data-stu-id="7b07e-222">String</span></span>|<span data-ttu-id="7b07e-223">Код продукта.</span><span class="sxs-lookup"><span data-stu-id="7b07e-223">The product code.</span></span>|
|<span data-ttu-id="7b07e-224">productVersion</span><span class="sxs-lookup"><span data-stu-id="7b07e-224">productVersion</span></span>|<span data-ttu-id="7b07e-225">String</span><span class="sxs-lookup"><span data-stu-id="7b07e-225">String</span></span>|<span data-ttu-id="7b07e-226">Версия бизнес-приложения, к которому применяется MSI Windows Mobile.</span><span class="sxs-lookup"><span data-stu-id="7b07e-226">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="7b07e-227">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="7b07e-227">ignoreVersionDetection</span></span>|<span data-ttu-id="7b07e-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b07e-228">Boolean</span></span>|<span data-ttu-id="7b07e-229">Логическое значение, позволяющее разрешить или запретить поиск установленного приложения по его версии.</span><span class="sxs-lookup"><span data-stu-id="7b07e-229">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="7b07e-230">Задайте значение true для бизнес-приложений MSI для Windows Mobile с функцией самостоятельного обновления.</span><span class="sxs-lookup"><span data-stu-id="7b07e-230">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="7b07e-231">identityVersion</span><span class="sxs-lookup"><span data-stu-id="7b07e-231">identityVersion</span></span>|<span data-ttu-id="7b07e-232">String</span><span class="sxs-lookup"><span data-stu-id="7b07e-232">String</span></span>|<span data-ttu-id="7b07e-233">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="7b07e-233">The identity version.</span></span>|
|<span data-ttu-id="7b07e-234">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="7b07e-234">useDeviceContext</span></span>|<span data-ttu-id="7b07e-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b07e-235">Boolean</span></span>|<span data-ttu-id="7b07e-236">Указывает, следует ли установить MSI с двойным режимом в контексте устройства.</span><span class="sxs-lookup"><span data-stu-id="7b07e-236">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="7b07e-237">Если задано значение true, приложение будет установлено для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="7b07e-237">If true, app will be installed for all users.</span></span> <span data-ttu-id="7b07e-238">Если задано значение false, приложение будет установлено для каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="7b07e-238">If false, app will be installed per-user.</span></span> <span data-ttu-id="7b07e-239">Если значение равно null, служба будет использовать стандартный контекст установки пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="7b07e-239">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="7b07e-240">В случае с двойным режимом MSI это значение по умолчанию будет иметь значение "на пользователя".</span><span class="sxs-lookup"><span data-stu-id="7b07e-240">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="7b07e-241">Не может быть задано для приложений с несдвоенным режимом.</span><span class="sxs-lookup"><span data-stu-id="7b07e-241">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="7b07e-242">После первоначального создания приложения его невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="7b07e-242">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="7b07e-243">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b07e-243">Response</span></span>
<span data-ttu-id="7b07e-244">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7b07e-244">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b07e-245">Пример</span><span class="sxs-lookup"><span data-stu-id="7b07e-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b07e-246">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b07e-246">Request</span></span>
<span data-ttu-id="7b07e-247">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b07e-247">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="7b07e-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b07e-248">Response</span></span>
<span data-ttu-id="7b07e-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b07e-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



