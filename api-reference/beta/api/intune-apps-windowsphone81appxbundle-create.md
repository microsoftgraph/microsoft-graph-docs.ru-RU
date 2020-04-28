---
title: Создание windowsPhone81AppXBundle
description: Создание нового объекта windowsPhone81AppXBundle.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b727c08d71e9ca6e9efd54b040fe7cac8f96e85d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43409275"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="41963-103">Создание windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="41963-103">Create windowsPhone81AppXBundle</span></span>

<span data-ttu-id="41963-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41963-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41963-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41963-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41963-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="41963-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41963-107">Создание нового объекта [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="41963-107">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41963-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="41963-108">Prerequisites</span></span>
<span data-ttu-id="41963-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41963-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41963-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41963-111">Permission type</span></span>|<span data-ttu-id="41963-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="41963-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41963-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41963-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41963-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41963-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="41963-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41963-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41963-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41963-116">Not supported.</span></span>|
|<span data-ttu-id="41963-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41963-117">Application</span></span>|<span data-ttu-id="41963-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41963-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41963-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41963-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="41963-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="41963-120">Request headers</span></span>
|<span data-ttu-id="41963-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41963-121">Header</span></span>|<span data-ttu-id="41963-122">Значение</span><span class="sxs-lookup"><span data-stu-id="41963-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41963-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41963-123">Authorization</span></span>|<span data-ttu-id="41963-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41963-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41963-125">Accept</span><span class="sxs-lookup"><span data-stu-id="41963-125">Accept</span></span>|<span data-ttu-id="41963-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41963-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41963-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="41963-127">Request body</span></span>
<span data-ttu-id="41963-128">В тексте запроса добавьте представление объекта windowsPhone81AppXBundle в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41963-128">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="41963-129">В следующей таблице приведены свойства, необходимые при создании windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="41963-129">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="41963-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="41963-130">Property</span></span>|<span data-ttu-id="41963-131">Тип</span><span class="sxs-lookup"><span data-stu-id="41963-131">Type</span></span>|<span data-ttu-id="41963-132">Описание</span><span class="sxs-lookup"><span data-stu-id="41963-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41963-133">id</span><span class="sxs-lookup"><span data-stu-id="41963-133">id</span></span>|<span data-ttu-id="41963-134">Строка</span><span class="sxs-lookup"><span data-stu-id="41963-134">String</span></span>|<span data-ttu-id="41963-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="41963-135">Key of the entity.</span></span> <span data-ttu-id="41963-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-137">displayName</span><span class="sxs-lookup"><span data-stu-id="41963-137">displayName</span></span>|<span data-ttu-id="41963-138">Строка</span><span class="sxs-lookup"><span data-stu-id="41963-138">String</span></span>|<span data-ttu-id="41963-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="41963-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="41963-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-141">description</span><span class="sxs-lookup"><span data-stu-id="41963-141">description</span></span>|<span data-ttu-id="41963-142">Строка</span><span class="sxs-lookup"><span data-stu-id="41963-142">String</span></span>|<span data-ttu-id="41963-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="41963-143">The description of the app.</span></span> <span data-ttu-id="41963-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-145">publisher</span><span class="sxs-lookup"><span data-stu-id="41963-145">publisher</span></span>|<span data-ttu-id="41963-146">String</span><span class="sxs-lookup"><span data-stu-id="41963-146">String</span></span>|<span data-ttu-id="41963-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="41963-147">The publisher of the app.</span></span> <span data-ttu-id="41963-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="41963-149">largeIcon</span></span>|[<span data-ttu-id="41963-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="41963-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="41963-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="41963-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="41963-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41963-153">createdDateTime</span></span>|<span data-ttu-id="41963-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41963-154">DateTimeOffset</span></span>|<span data-ttu-id="41963-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="41963-155">The date and time the app was created.</span></span> <span data-ttu-id="41963-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41963-157">lastModifiedDateTime</span></span>|<span data-ttu-id="41963-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41963-158">DateTimeOffset</span></span>|<span data-ttu-id="41963-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="41963-159">The date and time the app was last modified.</span></span> <span data-ttu-id="41963-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="41963-161">isFeatured</span></span>|<span data-ttu-id="41963-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="41963-162">Boolean</span></span>|<span data-ttu-id="41963-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="41963-164">privacyInformationUrl</span></span>|<span data-ttu-id="41963-165">String</span><span class="sxs-lookup"><span data-stu-id="41963-165">String</span></span>|<span data-ttu-id="41963-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="41963-166">The privacy statement Url.</span></span> <span data-ttu-id="41963-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="41963-168">informationUrl</span></span>|<span data-ttu-id="41963-169">String</span><span class="sxs-lookup"><span data-stu-id="41963-169">String</span></span>|<span data-ttu-id="41963-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="41963-170">The more information Url.</span></span> <span data-ttu-id="41963-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-172">owner</span><span class="sxs-lookup"><span data-stu-id="41963-172">owner</span></span>|<span data-ttu-id="41963-173">String</span><span class="sxs-lookup"><span data-stu-id="41963-173">String</span></span>|<span data-ttu-id="41963-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="41963-174">The owner of the app.</span></span> <span data-ttu-id="41963-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-176">developer</span><span class="sxs-lookup"><span data-stu-id="41963-176">developer</span></span>|<span data-ttu-id="41963-177">String</span><span class="sxs-lookup"><span data-stu-id="41963-177">String</span></span>|<span data-ttu-id="41963-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="41963-178">The developer of the app.</span></span> <span data-ttu-id="41963-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-180">notes</span><span class="sxs-lookup"><span data-stu-id="41963-180">notes</span></span>|<span data-ttu-id="41963-181">String</span><span class="sxs-lookup"><span data-stu-id="41963-181">String</span></span>|<span data-ttu-id="41963-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="41963-182">Notes for the app.</span></span> <span data-ttu-id="41963-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="41963-184">uploadState</span></span>|<span data-ttu-id="41963-185">Int32</span><span class="sxs-lookup"><span data-stu-id="41963-185">Int32</span></span>|<span data-ttu-id="41963-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="41963-186">The upload state.</span></span> <span data-ttu-id="41963-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="41963-188">publishingState</span></span>|[<span data-ttu-id="41963-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="41963-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="41963-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="41963-190">The publishing state for the app.</span></span> <span data-ttu-id="41963-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="41963-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="41963-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="41963-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="41963-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="41963-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="41963-194">isAssigned</span></span>|<span data-ttu-id="41963-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="41963-195">Boolean</span></span>|<span data-ttu-id="41963-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="41963-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="41963-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="41963-198">roleScopeTagIds</span></span>|<span data-ttu-id="41963-199">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="41963-199">String collection</span></span>|<span data-ttu-id="41963-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="41963-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="41963-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="41963-202">dependentAppCount</span></span>|<span data-ttu-id="41963-203">Int32</span><span class="sxs-lookup"><span data-stu-id="41963-203">Int32</span></span>|<span data-ttu-id="41963-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="41963-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="41963-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="41963-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="41963-206">committedContentVersion</span></span>|<span data-ttu-id="41963-207">String</span><span class="sxs-lookup"><span data-stu-id="41963-207">String</span></span>|<span data-ttu-id="41963-208">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="41963-208">The internal committed content version.</span></span> <span data-ttu-id="41963-209">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="41963-210">fileName</span><span class="sxs-lookup"><span data-stu-id="41963-210">fileName</span></span>|<span data-ttu-id="41963-211">String</span><span class="sxs-lookup"><span data-stu-id="41963-211">String</span></span>|<span data-ttu-id="41963-212">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="41963-212">The name of the main Lob application file.</span></span> <span data-ttu-id="41963-213">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="41963-214">size</span><span class="sxs-lookup"><span data-stu-id="41963-214">size</span></span>|<span data-ttu-id="41963-215">Int64</span><span class="sxs-lookup"><span data-stu-id="41963-215">Int64</span></span>|<span data-ttu-id="41963-216">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="41963-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="41963-217">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="41963-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="41963-218">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="41963-218">applicableArchitectures</span></span>|[<span data-ttu-id="41963-219">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="41963-219">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="41963-220">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="41963-220">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="41963-221">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="41963-221">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="41963-222">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="41963-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="41963-223">identityName</span><span class="sxs-lookup"><span data-stu-id="41963-223">identityName</span></span>|<span data-ttu-id="41963-224">String</span><span class="sxs-lookup"><span data-stu-id="41963-224">String</span></span>|<span data-ttu-id="41963-225">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="41963-225">The Identity Name.</span></span> <span data-ttu-id="41963-226">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="41963-226">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="41963-227">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="41963-227">identityPublisherHash</span></span>|<span data-ttu-id="41963-228">String</span><span class="sxs-lookup"><span data-stu-id="41963-228">String</span></span>|<span data-ttu-id="41963-229">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="41963-229">The Identity Publisher Hash.</span></span> <span data-ttu-id="41963-230">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="41963-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="41963-231">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="41963-231">identityResourceIdentifier</span></span>|<span data-ttu-id="41963-232">String</span><span class="sxs-lookup"><span data-stu-id="41963-232">String</span></span>|<span data-ttu-id="41963-233">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="41963-233">The Identity Resource Identifier.</span></span> <span data-ttu-id="41963-234">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="41963-234">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="41963-235">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="41963-235">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="41963-236">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="41963-236">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="41963-237">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="41963-237">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="41963-238">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="41963-238">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="41963-239">фонепродуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="41963-239">phoneProductIdentifier</span></span>|<span data-ttu-id="41963-240">String</span><span class="sxs-lookup"><span data-stu-id="41963-240">String</span></span>|<span data-ttu-id="41963-241">Идентификатор телефонного продукта.</span><span class="sxs-lookup"><span data-stu-id="41963-241">The Phone Product Identifier.</span></span> <span data-ttu-id="41963-242">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="41963-242">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="41963-243">фонепублишерид</span><span class="sxs-lookup"><span data-stu-id="41963-243">phonePublisherId</span></span>|<span data-ttu-id="41963-244">String</span><span class="sxs-lookup"><span data-stu-id="41963-244">String</span></span>|<span data-ttu-id="41963-245">Идентификатор издателя телефона. наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="41963-245">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="41963-246">identityVersion</span><span class="sxs-lookup"><span data-stu-id="41963-246">identityVersion</span></span>|<span data-ttu-id="41963-247">String</span><span class="sxs-lookup"><span data-stu-id="41963-247">String</span></span>|<span data-ttu-id="41963-248">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="41963-248">The identity version.</span></span> <span data-ttu-id="41963-249">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="41963-249">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="41963-250">аппкспаккажеинформатионлист</span><span class="sxs-lookup"><span data-stu-id="41963-250">appXPackageInformationList</span></span>|<span data-ttu-id="41963-251">Коллекция [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="41963-251">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="41963-252">Список сведений о пакете AppX.</span><span class="sxs-lookup"><span data-stu-id="41963-252">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="41963-253">Ответ</span><span class="sxs-lookup"><span data-stu-id="41963-253">Response</span></span>
<span data-ttu-id="41963-254">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="41963-254">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41963-255">Пример</span><span class="sxs-lookup"><span data-stu-id="41963-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="41963-256">Запрос</span><span class="sxs-lookup"><span data-stu-id="41963-256">Request</span></span>
<span data-ttu-id="41963-257">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41963-257">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2311

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true,
        "v10_1809": true,
        "v10_1903": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="41963-258">Отклик</span><span class="sxs-lookup"><span data-stu-id="41963-258">Response</span></span>
<span data-ttu-id="41963-p129">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="41963-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2483

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true,
        "v10_1809": true,
        "v10_1903": true
      }
    }
  ]
}
```



