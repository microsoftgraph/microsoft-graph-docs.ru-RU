---
title: Создание windowsPhone81AppXBundle
description: Создание нового объекта windowsPhone81AppXBundle.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e0c59bcfc3a976ea0ec077444f28e854e2da465
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798203"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="47d97-103">Создание windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="47d97-103">Create windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="47d97-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47d97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47d97-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47d97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47d97-106">Создание нового объекта [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="47d97-106">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47d97-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="47d97-107">Prerequisites</span></span>
<span data-ttu-id="47d97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47d97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47d97-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47d97-110">Permission type</span></span>|<span data-ttu-id="47d97-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47d97-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47d97-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47d97-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47d97-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d97-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="47d97-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47d97-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47d97-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47d97-115">Not supported.</span></span>|
|<span data-ttu-id="47d97-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47d97-116">Application</span></span>|<span data-ttu-id="47d97-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47d97-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47d97-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47d97-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="47d97-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47d97-119">Request headers</span></span>
|<span data-ttu-id="47d97-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47d97-120">Header</span></span>|<span data-ttu-id="47d97-121">Значение</span><span class="sxs-lookup"><span data-stu-id="47d97-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47d97-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47d97-122">Authorization</span></span>|<span data-ttu-id="47d97-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47d97-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47d97-124">Accept</span><span class="sxs-lookup"><span data-stu-id="47d97-124">Accept</span></span>|<span data-ttu-id="47d97-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47d97-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47d97-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47d97-126">Request body</span></span>
<span data-ttu-id="47d97-127">В тексте запроса добавьте представление объекта windowsPhone81AppXBundle в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47d97-127">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="47d97-128">В следующей таблице приведены свойства, необходимые при создании windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="47d97-128">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="47d97-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="47d97-129">Property</span></span>|<span data-ttu-id="47d97-130">Тип</span><span class="sxs-lookup"><span data-stu-id="47d97-130">Type</span></span>|<span data-ttu-id="47d97-131">Описание</span><span class="sxs-lookup"><span data-stu-id="47d97-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47d97-132">id</span><span class="sxs-lookup"><span data-stu-id="47d97-132">id</span></span>|<span data-ttu-id="47d97-133">Строка</span><span class="sxs-lookup"><span data-stu-id="47d97-133">String</span></span>|<span data-ttu-id="47d97-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="47d97-134">Key of the entity.</span></span> <span data-ttu-id="47d97-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-136">displayName</span><span class="sxs-lookup"><span data-stu-id="47d97-136">displayName</span></span>|<span data-ttu-id="47d97-137">Строка</span><span class="sxs-lookup"><span data-stu-id="47d97-137">String</span></span>|<span data-ttu-id="47d97-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="47d97-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="47d97-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-140">description</span><span class="sxs-lookup"><span data-stu-id="47d97-140">description</span></span>|<span data-ttu-id="47d97-141">String</span><span class="sxs-lookup"><span data-stu-id="47d97-141">String</span></span>|<span data-ttu-id="47d97-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="47d97-142">The description of the app.</span></span> <span data-ttu-id="47d97-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-144">publisher</span><span class="sxs-lookup"><span data-stu-id="47d97-144">publisher</span></span>|<span data-ttu-id="47d97-145">String</span><span class="sxs-lookup"><span data-stu-id="47d97-145">String</span></span>|<span data-ttu-id="47d97-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="47d97-146">The publisher of the app.</span></span> <span data-ttu-id="47d97-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="47d97-148">largeIcon</span></span>|[<span data-ttu-id="47d97-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="47d97-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="47d97-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="47d97-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="47d97-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47d97-152">createdDateTime</span></span>|<span data-ttu-id="47d97-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47d97-153">DateTimeOffset</span></span>|<span data-ttu-id="47d97-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="47d97-154">The date and time the app was created.</span></span> <span data-ttu-id="47d97-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47d97-156">lastModifiedDateTime</span></span>|<span data-ttu-id="47d97-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47d97-157">DateTimeOffset</span></span>|<span data-ttu-id="47d97-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="47d97-158">The date and time the app was last modified.</span></span> <span data-ttu-id="47d97-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="47d97-160">isFeatured</span></span>|<span data-ttu-id="47d97-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="47d97-161">Boolean</span></span>|<span data-ttu-id="47d97-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="47d97-163">privacyInformationUrl</span></span>|<span data-ttu-id="47d97-164">String</span><span class="sxs-lookup"><span data-stu-id="47d97-164">String</span></span>|<span data-ttu-id="47d97-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="47d97-165">The privacy statement Url.</span></span> <span data-ttu-id="47d97-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="47d97-167">informationUrl</span></span>|<span data-ttu-id="47d97-168">String</span><span class="sxs-lookup"><span data-stu-id="47d97-168">String</span></span>|<span data-ttu-id="47d97-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="47d97-169">The more information Url.</span></span> <span data-ttu-id="47d97-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-171">owner</span><span class="sxs-lookup"><span data-stu-id="47d97-171">owner</span></span>|<span data-ttu-id="47d97-172">String</span><span class="sxs-lookup"><span data-stu-id="47d97-172">String</span></span>|<span data-ttu-id="47d97-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="47d97-173">The owner of the app.</span></span> <span data-ttu-id="47d97-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-175">developer</span><span class="sxs-lookup"><span data-stu-id="47d97-175">developer</span></span>|<span data-ttu-id="47d97-176">String</span><span class="sxs-lookup"><span data-stu-id="47d97-176">String</span></span>|<span data-ttu-id="47d97-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="47d97-177">The developer of the app.</span></span> <span data-ttu-id="47d97-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-179">notes</span><span class="sxs-lookup"><span data-stu-id="47d97-179">notes</span></span>|<span data-ttu-id="47d97-180">String</span><span class="sxs-lookup"><span data-stu-id="47d97-180">String</span></span>|<span data-ttu-id="47d97-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="47d97-181">Notes for the app.</span></span> <span data-ttu-id="47d97-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="47d97-183">uploadState</span></span>|<span data-ttu-id="47d97-184">Int32</span><span class="sxs-lookup"><span data-stu-id="47d97-184">Int32</span></span>|<span data-ttu-id="47d97-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="47d97-185">The upload state.</span></span> <span data-ttu-id="47d97-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="47d97-187">publishingState</span></span>|[<span data-ttu-id="47d97-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="47d97-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="47d97-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="47d97-189">The publishing state for the app.</span></span> <span data-ttu-id="47d97-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="47d97-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="47d97-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="47d97-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="47d97-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="47d97-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="47d97-193">isAssigned</span></span>|<span data-ttu-id="47d97-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="47d97-194">Boolean</span></span>|<span data-ttu-id="47d97-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="47d97-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="47d97-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="47d97-197">roleScopeTagIds</span></span>|<span data-ttu-id="47d97-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="47d97-198">String collection</span></span>|<span data-ttu-id="47d97-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="47d97-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="47d97-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="47d97-201">dependentAppCount</span></span>|<span data-ttu-id="47d97-202">Int32</span><span class="sxs-lookup"><span data-stu-id="47d97-202">Int32</span></span>|<span data-ttu-id="47d97-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="47d97-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="47d97-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47d97-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="47d97-205">committedContentVersion</span></span>|<span data-ttu-id="47d97-206">String</span><span class="sxs-lookup"><span data-stu-id="47d97-206">String</span></span>|<span data-ttu-id="47d97-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="47d97-207">The internal committed content version.</span></span> <span data-ttu-id="47d97-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="47d97-209">fileName</span><span class="sxs-lookup"><span data-stu-id="47d97-209">fileName</span></span>|<span data-ttu-id="47d97-210">String</span><span class="sxs-lookup"><span data-stu-id="47d97-210">String</span></span>|<span data-ttu-id="47d97-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="47d97-211">The name of the main Lob application file.</span></span> <span data-ttu-id="47d97-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="47d97-213">size</span><span class="sxs-lookup"><span data-stu-id="47d97-213">size</span></span>|<span data-ttu-id="47d97-214">Int64</span><span class="sxs-lookup"><span data-stu-id="47d97-214">Int64</span></span>|<span data-ttu-id="47d97-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="47d97-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="47d97-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="47d97-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="47d97-217">applicableArchitectures</span></span>|[<span data-ttu-id="47d97-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="47d97-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="47d97-219">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="47d97-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="47d97-220">НаСледуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="47d97-220">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="47d97-221">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="47d97-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="47d97-222">identityName</span><span class="sxs-lookup"><span data-stu-id="47d97-222">identityName</span></span>|<span data-ttu-id="47d97-223">String</span><span class="sxs-lookup"><span data-stu-id="47d97-223">String</span></span>|<span data-ttu-id="47d97-224">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="47d97-224">The Identity Name.</span></span> <span data-ttu-id="47d97-225">НаСледуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="47d97-225">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="47d97-226">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="47d97-226">identityPublisherHash</span></span>|<span data-ttu-id="47d97-227">String</span><span class="sxs-lookup"><span data-stu-id="47d97-227">String</span></span>|<span data-ttu-id="47d97-228">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="47d97-228">The Identity Publisher Hash.</span></span> <span data-ttu-id="47d97-229">НаСледуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="47d97-229">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="47d97-230">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="47d97-230">identityResourceIdentifier</span></span>|<span data-ttu-id="47d97-231">String</span><span class="sxs-lookup"><span data-stu-id="47d97-231">String</span></span>|<span data-ttu-id="47d97-232">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="47d97-232">The Identity Resource Identifier.</span></span> <span data-ttu-id="47d97-233">НаСледуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="47d97-233">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="47d97-234">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="47d97-234">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="47d97-235">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="47d97-235">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="47d97-236">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="47d97-236">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="47d97-237">НаСледуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="47d97-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="47d97-238">Фонепродуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="47d97-238">phoneProductIdentifier</span></span>|<span data-ttu-id="47d97-239">String</span><span class="sxs-lookup"><span data-stu-id="47d97-239">String</span></span>|<span data-ttu-id="47d97-240">Идентификатор телефонного продукта.</span><span class="sxs-lookup"><span data-stu-id="47d97-240">The Phone Product Identifier.</span></span> <span data-ttu-id="47d97-241">НаСледуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="47d97-241">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="47d97-242">Фонепублишерид</span><span class="sxs-lookup"><span data-stu-id="47d97-242">phonePublisherId</span></span>|<span data-ttu-id="47d97-243">String</span><span class="sxs-lookup"><span data-stu-id="47d97-243">String</span></span>|<span data-ttu-id="47d97-244">Идентификатор издателя телефона. наСледуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="47d97-244">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="47d97-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="47d97-245">identityVersion</span></span>|<span data-ttu-id="47d97-246">String</span><span class="sxs-lookup"><span data-stu-id="47d97-246">String</span></span>|<span data-ttu-id="47d97-247">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="47d97-247">The identity version.</span></span> <span data-ttu-id="47d97-248">НаСледуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="47d97-248">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="47d97-249">Аппкспаккажеинформатионлист</span><span class="sxs-lookup"><span data-stu-id="47d97-249">appXPackageInformationList</span></span>|<span data-ttu-id="47d97-250">Коллекция [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="47d97-250">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="47d97-251">Список сведений о пакете AppX.</span><span class="sxs-lookup"><span data-stu-id="47d97-251">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="47d97-252">Отклик</span><span class="sxs-lookup"><span data-stu-id="47d97-252">Response</span></span>
<span data-ttu-id="47d97-253">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47d97-253">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47d97-254">Пример</span><span class="sxs-lookup"><span data-stu-id="47d97-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="47d97-255">Запрос</span><span class="sxs-lookup"><span data-stu-id="47d97-255">Request</span></span>
<span data-ttu-id="47d97-256">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47d97-256">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2211

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
    "v10_1803": true
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
        "v10_1803": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="47d97-257">Отклик</span><span class="sxs-lookup"><span data-stu-id="47d97-257">Response</span></span>
<span data-ttu-id="47d97-p129">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47d97-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2383

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
    "v10_1803": true
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
        "v10_1803": true
      }
    }
  ]
}
```





