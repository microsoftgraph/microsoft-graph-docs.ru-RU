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
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="96d7c-103">Создание windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="96d7c-103">Create windowsPhone81AppXBundle</span></span>

<span data-ttu-id="96d7c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96d7c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96d7c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96d7c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96d7c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="96d7c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96d7c-107">Создание нового объекта [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="96d7c-107">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96d7c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="96d7c-108">Prerequisites</span></span>
<span data-ttu-id="96d7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96d7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96d7c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96d7c-111">Permission type</span></span>|<span data-ttu-id="96d7c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="96d7c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96d7c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96d7c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96d7c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96d7c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="96d7c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96d7c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96d7c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96d7c-116">Not supported.</span></span>|
|<span data-ttu-id="96d7c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="96d7c-117">Application</span></span>|<span data-ttu-id="96d7c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96d7c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96d7c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96d7c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="96d7c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="96d7c-120">Request headers</span></span>
|<span data-ttu-id="96d7c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96d7c-121">Header</span></span>|<span data-ttu-id="96d7c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="96d7c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96d7c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96d7c-123">Authorization</span></span>|<span data-ttu-id="96d7c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96d7c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96d7c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="96d7c-125">Accept</span></span>|<span data-ttu-id="96d7c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96d7c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96d7c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96d7c-127">Request body</span></span>
<span data-ttu-id="96d7c-128">В тексте запроса добавьте представление объекта windowsPhone81AppXBundle в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96d7c-128">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="96d7c-129">В следующей таблице приведены свойства, необходимые при создании windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="96d7c-129">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="96d7c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="96d7c-130">Property</span></span>|<span data-ttu-id="96d7c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="96d7c-131">Type</span></span>|<span data-ttu-id="96d7c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="96d7c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96d7c-133">id</span><span class="sxs-lookup"><span data-stu-id="96d7c-133">id</span></span>|<span data-ttu-id="96d7c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="96d7c-134">String</span></span>|<span data-ttu-id="96d7c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="96d7c-135">Key of the entity.</span></span> <span data-ttu-id="96d7c-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="96d7c-137">displayName</span></span>|<span data-ttu-id="96d7c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="96d7c-138">String</span></span>|<span data-ttu-id="96d7c-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="96d7c-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="96d7c-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-141">description</span><span class="sxs-lookup"><span data-stu-id="96d7c-141">description</span></span>|<span data-ttu-id="96d7c-142">Строка</span><span class="sxs-lookup"><span data-stu-id="96d7c-142">String</span></span>|<span data-ttu-id="96d7c-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="96d7c-143">The description of the app.</span></span> <span data-ttu-id="96d7c-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-145">publisher</span><span class="sxs-lookup"><span data-stu-id="96d7c-145">publisher</span></span>|<span data-ttu-id="96d7c-146">String</span><span class="sxs-lookup"><span data-stu-id="96d7c-146">String</span></span>|<span data-ttu-id="96d7c-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="96d7c-147">The publisher of the app.</span></span> <span data-ttu-id="96d7c-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="96d7c-149">largeIcon</span></span>|[<span data-ttu-id="96d7c-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="96d7c-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="96d7c-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="96d7c-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="96d7c-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96d7c-153">createdDateTime</span></span>|<span data-ttu-id="96d7c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96d7c-154">DateTimeOffset</span></span>|<span data-ttu-id="96d7c-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="96d7c-155">The date and time the app was created.</span></span> <span data-ttu-id="96d7c-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96d7c-157">lastModifiedDateTime</span></span>|<span data-ttu-id="96d7c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96d7c-158">DateTimeOffset</span></span>|<span data-ttu-id="96d7c-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="96d7c-159">The date and time the app was last modified.</span></span> <span data-ttu-id="96d7c-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="96d7c-161">isFeatured</span></span>|<span data-ttu-id="96d7c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="96d7c-162">Boolean</span></span>|<span data-ttu-id="96d7c-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="96d7c-164">privacyInformationUrl</span></span>|<span data-ttu-id="96d7c-165">String</span><span class="sxs-lookup"><span data-stu-id="96d7c-165">String</span></span>|<span data-ttu-id="96d7c-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="96d7c-166">The privacy statement Url.</span></span> <span data-ttu-id="96d7c-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="96d7c-168">informationUrl</span></span>|<span data-ttu-id="96d7c-169">String</span><span class="sxs-lookup"><span data-stu-id="96d7c-169">String</span></span>|<span data-ttu-id="96d7c-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="96d7c-170">The more information Url.</span></span> <span data-ttu-id="96d7c-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-172">owner</span><span class="sxs-lookup"><span data-stu-id="96d7c-172">owner</span></span>|<span data-ttu-id="96d7c-173">String</span><span class="sxs-lookup"><span data-stu-id="96d7c-173">String</span></span>|<span data-ttu-id="96d7c-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="96d7c-174">The owner of the app.</span></span> <span data-ttu-id="96d7c-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-176">developer</span><span class="sxs-lookup"><span data-stu-id="96d7c-176">developer</span></span>|<span data-ttu-id="96d7c-177">String</span><span class="sxs-lookup"><span data-stu-id="96d7c-177">String</span></span>|<span data-ttu-id="96d7c-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="96d7c-178">The developer of the app.</span></span> <span data-ttu-id="96d7c-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-180">notes</span><span class="sxs-lookup"><span data-stu-id="96d7c-180">notes</span></span>|<span data-ttu-id="96d7c-181">String</span><span class="sxs-lookup"><span data-stu-id="96d7c-181">String</span></span>|<span data-ttu-id="96d7c-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="96d7c-182">Notes for the app.</span></span> <span data-ttu-id="96d7c-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="96d7c-184">uploadState</span></span>|<span data-ttu-id="96d7c-185">Int32</span><span class="sxs-lookup"><span data-stu-id="96d7c-185">Int32</span></span>|<span data-ttu-id="96d7c-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="96d7c-186">The upload state.</span></span> <span data-ttu-id="96d7c-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="96d7c-188">publishingState</span></span>|[<span data-ttu-id="96d7c-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="96d7c-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="96d7c-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="96d7c-190">The publishing state for the app.</span></span> <span data-ttu-id="96d7c-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="96d7c-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="96d7c-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="96d7c-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="96d7c-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="96d7c-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="96d7c-194">isAssigned</span></span>|<span data-ttu-id="96d7c-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="96d7c-195">Boolean</span></span>|<span data-ttu-id="96d7c-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="96d7c-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="96d7c-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="96d7c-198">roleScopeTagIds</span></span>|<span data-ttu-id="96d7c-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="96d7c-199">String collection</span></span>|<span data-ttu-id="96d7c-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="96d7c-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="96d7c-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="96d7c-202">dependentAppCount</span></span>|<span data-ttu-id="96d7c-203">Int32</span><span class="sxs-lookup"><span data-stu-id="96d7c-203">Int32</span></span>|<span data-ttu-id="96d7c-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="96d7c-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="96d7c-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="96d7c-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="96d7c-206">committedContentVersion</span></span>|<span data-ttu-id="96d7c-207">String</span><span class="sxs-lookup"><span data-stu-id="96d7c-207">String</span></span>|<span data-ttu-id="96d7c-208">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="96d7c-208">The internal committed content version.</span></span> <span data-ttu-id="96d7c-209">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="96d7c-210">fileName</span><span class="sxs-lookup"><span data-stu-id="96d7c-210">fileName</span></span>|<span data-ttu-id="96d7c-211">String</span><span class="sxs-lookup"><span data-stu-id="96d7c-211">String</span></span>|<span data-ttu-id="96d7c-212">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="96d7c-212">The name of the main Lob application file.</span></span> <span data-ttu-id="96d7c-213">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="96d7c-214">size</span><span class="sxs-lookup"><span data-stu-id="96d7c-214">size</span></span>|<span data-ttu-id="96d7c-215">Int64</span><span class="sxs-lookup"><span data-stu-id="96d7c-215">Int64</span></span>|<span data-ttu-id="96d7c-216">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="96d7c-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="96d7c-217">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="96d7c-218">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="96d7c-218">applicableArchitectures</span></span>|[<span data-ttu-id="96d7c-219">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="96d7c-219">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="96d7c-220">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="96d7c-220">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="96d7c-221">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="96d7c-221">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="96d7c-222">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="96d7c-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="96d7c-223">identityName</span><span class="sxs-lookup"><span data-stu-id="96d7c-223">identityName</span></span>|<span data-ttu-id="96d7c-224">String</span><span class="sxs-lookup"><span data-stu-id="96d7c-224">String</span></span>|<span data-ttu-id="96d7c-225">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="96d7c-225">The Identity Name.</span></span> <span data-ttu-id="96d7c-226">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="96d7c-226">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="96d7c-227">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="96d7c-227">identityPublisherHash</span></span>|<span data-ttu-id="96d7c-228">String</span><span class="sxs-lookup"><span data-stu-id="96d7c-228">String</span></span>|<span data-ttu-id="96d7c-229">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="96d7c-229">The Identity Publisher Hash.</span></span> <span data-ttu-id="96d7c-230">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="96d7c-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="96d7c-231">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="96d7c-231">identityResourceIdentifier</span></span>|<span data-ttu-id="96d7c-232">String</span><span class="sxs-lookup"><span data-stu-id="96d7c-232">String</span></span>|<span data-ttu-id="96d7c-233">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="96d7c-233">The Identity Resource Identifier.</span></span> <span data-ttu-id="96d7c-234">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="96d7c-234">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="96d7c-235">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="96d7c-235">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="96d7c-236">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="96d7c-236">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="96d7c-237">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="96d7c-237">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="96d7c-238">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="96d7c-238">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="96d7c-239">фонепродуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="96d7c-239">phoneProductIdentifier</span></span>|<span data-ttu-id="96d7c-240">String</span><span class="sxs-lookup"><span data-stu-id="96d7c-240">String</span></span>|<span data-ttu-id="96d7c-241">Идентификатор телефонного продукта.</span><span class="sxs-lookup"><span data-stu-id="96d7c-241">The Phone Product Identifier.</span></span> <span data-ttu-id="96d7c-242">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="96d7c-242">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="96d7c-243">фонепублишерид</span><span class="sxs-lookup"><span data-stu-id="96d7c-243">phonePublisherId</span></span>|<span data-ttu-id="96d7c-244">String</span><span class="sxs-lookup"><span data-stu-id="96d7c-244">String</span></span>|<span data-ttu-id="96d7c-245">Идентификатор издателя телефона. наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="96d7c-245">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="96d7c-246">identityVersion</span><span class="sxs-lookup"><span data-stu-id="96d7c-246">identityVersion</span></span>|<span data-ttu-id="96d7c-247">String</span><span class="sxs-lookup"><span data-stu-id="96d7c-247">String</span></span>|<span data-ttu-id="96d7c-248">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="96d7c-248">The identity version.</span></span> <span data-ttu-id="96d7c-249">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="96d7c-249">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="96d7c-250">аппкспаккажеинформатионлист</span><span class="sxs-lookup"><span data-stu-id="96d7c-250">appXPackageInformationList</span></span>|<span data-ttu-id="96d7c-251">Коллекция [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="96d7c-251">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="96d7c-252">Список сведений о пакете AppX.</span><span class="sxs-lookup"><span data-stu-id="96d7c-252">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="96d7c-253">Отклик</span><span class="sxs-lookup"><span data-stu-id="96d7c-253">Response</span></span>
<span data-ttu-id="96d7c-254">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96d7c-254">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96d7c-255">Пример</span><span class="sxs-lookup"><span data-stu-id="96d7c-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="96d7c-256">Запрос</span><span class="sxs-lookup"><span data-stu-id="96d7c-256">Request</span></span>
<span data-ttu-id="96d7c-257">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96d7c-257">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="96d7c-258">Отклик</span><span class="sxs-lookup"><span data-stu-id="96d7c-258">Response</span></span>
<span data-ttu-id="96d7c-p129">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96d7c-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



