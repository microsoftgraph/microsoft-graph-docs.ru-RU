---
title: Create windowsMobileMSI
description: Создание объекта windowsMobileMSI.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d077ce9865887aace9412b8b535655ebd077e294
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450547"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="6aed8-103">Create windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="6aed8-103">Create windowsMobileMSI</span></span>

<span data-ttu-id="6aed8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6aed8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6aed8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aed8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6aed8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6aed8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aed8-107">Создание объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-107">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6aed8-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6aed8-108">Prerequisites</span></span>
<span data-ttu-id="6aed8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6aed8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aed8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6aed8-111">Permission type</span></span>|<span data-ttu-id="6aed8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6aed8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6aed8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6aed8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6aed8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aed8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6aed8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6aed8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6aed8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aed8-116">Not supported.</span></span>|
|<span data-ttu-id="6aed8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6aed8-117">Application</span></span>|<span data-ttu-id="6aed8-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aed8-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6aed8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6aed8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6aed8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6aed8-120">Request headers</span></span>
|<span data-ttu-id="6aed8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6aed8-121">Header</span></span>|<span data-ttu-id="6aed8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6aed8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6aed8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6aed8-123">Authorization</span></span>|<span data-ttu-id="6aed8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6aed8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6aed8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6aed8-125">Accept</span></span>|<span data-ttu-id="6aed8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6aed8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aed8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6aed8-127">Request body</span></span>
<span data-ttu-id="6aed8-128">В тексте запроса добавьте представление объекта windowsMobileMSI в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6aed8-128">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="6aed8-129">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="6aed8-129">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="6aed8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6aed8-130">Property</span></span>|<span data-ttu-id="6aed8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6aed8-131">Type</span></span>|<span data-ttu-id="6aed8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6aed8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6aed8-133">id</span><span class="sxs-lookup"><span data-stu-id="6aed8-133">id</span></span>|<span data-ttu-id="6aed8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6aed8-134">String</span></span>|<span data-ttu-id="6aed8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6aed8-135">Key of the entity.</span></span> <span data-ttu-id="6aed8-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6aed8-137">displayName</span></span>|<span data-ttu-id="6aed8-138">Строка</span><span class="sxs-lookup"><span data-stu-id="6aed8-138">String</span></span>|<span data-ttu-id="6aed8-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="6aed8-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6aed8-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-141">description</span><span class="sxs-lookup"><span data-stu-id="6aed8-141">description</span></span>|<span data-ttu-id="6aed8-142">Строка</span><span class="sxs-lookup"><span data-stu-id="6aed8-142">String</span></span>|<span data-ttu-id="6aed8-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="6aed8-143">The description of the app.</span></span> <span data-ttu-id="6aed8-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-145">publisher</span><span class="sxs-lookup"><span data-stu-id="6aed8-145">publisher</span></span>|<span data-ttu-id="6aed8-146">String</span><span class="sxs-lookup"><span data-stu-id="6aed8-146">String</span></span>|<span data-ttu-id="6aed8-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="6aed8-147">The publisher of the app.</span></span> <span data-ttu-id="6aed8-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6aed8-149">largeIcon</span></span>|[<span data-ttu-id="6aed8-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6aed8-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6aed8-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="6aed8-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6aed8-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6aed8-153">createdDateTime</span></span>|<span data-ttu-id="6aed8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6aed8-154">DateTimeOffset</span></span>|<span data-ttu-id="6aed8-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="6aed8-155">The date and time the app was created.</span></span> <span data-ttu-id="6aed8-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6aed8-157">lastModifiedDateTime</span></span>|<span data-ttu-id="6aed8-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6aed8-158">DateTimeOffset</span></span>|<span data-ttu-id="6aed8-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="6aed8-159">The date and time the app was last modified.</span></span> <span data-ttu-id="6aed8-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6aed8-161">isFeatured</span></span>|<span data-ttu-id="6aed8-162">Логический</span><span class="sxs-lookup"><span data-stu-id="6aed8-162">Boolean</span></span>|<span data-ttu-id="6aed8-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6aed8-164">privacyInformationUrl</span></span>|<span data-ttu-id="6aed8-165">String</span><span class="sxs-lookup"><span data-stu-id="6aed8-165">String</span></span>|<span data-ttu-id="6aed8-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="6aed8-166">The privacy statement Url.</span></span> <span data-ttu-id="6aed8-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6aed8-168">informationUrl</span></span>|<span data-ttu-id="6aed8-169">String</span><span class="sxs-lookup"><span data-stu-id="6aed8-169">String</span></span>|<span data-ttu-id="6aed8-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="6aed8-170">The more information Url.</span></span> <span data-ttu-id="6aed8-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-172">owner</span><span class="sxs-lookup"><span data-stu-id="6aed8-172">owner</span></span>|<span data-ttu-id="6aed8-173">String</span><span class="sxs-lookup"><span data-stu-id="6aed8-173">String</span></span>|<span data-ttu-id="6aed8-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="6aed8-174">The owner of the app.</span></span> <span data-ttu-id="6aed8-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-176">developer</span><span class="sxs-lookup"><span data-stu-id="6aed8-176">developer</span></span>|<span data-ttu-id="6aed8-177">String</span><span class="sxs-lookup"><span data-stu-id="6aed8-177">String</span></span>|<span data-ttu-id="6aed8-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="6aed8-178">The developer of the app.</span></span> <span data-ttu-id="6aed8-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-180">notes</span><span class="sxs-lookup"><span data-stu-id="6aed8-180">notes</span></span>|<span data-ttu-id="6aed8-181">String</span><span class="sxs-lookup"><span data-stu-id="6aed8-181">String</span></span>|<span data-ttu-id="6aed8-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="6aed8-182">Notes for the app.</span></span> <span data-ttu-id="6aed8-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="6aed8-184">uploadState</span></span>|<span data-ttu-id="6aed8-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6aed8-185">Int32</span></span>|<span data-ttu-id="6aed8-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="6aed8-186">The upload state.</span></span> <span data-ttu-id="6aed8-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="6aed8-188">publishingState</span></span>|[<span data-ttu-id="6aed8-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="6aed8-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6aed8-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="6aed8-190">The publishing state for the app.</span></span> <span data-ttu-id="6aed8-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="6aed8-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6aed8-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="6aed8-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6aed8-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6aed8-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6aed8-194">isAssigned</span></span>|<span data-ttu-id="6aed8-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aed8-195">Boolean</span></span>|<span data-ttu-id="6aed8-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="6aed8-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6aed8-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6aed8-198">roleScopeTagIds</span></span>|<span data-ttu-id="6aed8-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6aed8-199">String collection</span></span>|<span data-ttu-id="6aed8-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="6aed8-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6aed8-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="6aed8-202">dependentAppCount</span></span>|<span data-ttu-id="6aed8-203">Int32</span><span class="sxs-lookup"><span data-stu-id="6aed8-203">Int32</span></span>|<span data-ttu-id="6aed8-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="6aed8-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="6aed8-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6aed8-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="6aed8-206">committedContentVersion</span></span>|<span data-ttu-id="6aed8-207">String</span><span class="sxs-lookup"><span data-stu-id="6aed8-207">String</span></span>|<span data-ttu-id="6aed8-208">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="6aed8-208">The internal committed content version.</span></span> <span data-ttu-id="6aed8-209">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6aed8-210">fileName</span><span class="sxs-lookup"><span data-stu-id="6aed8-210">fileName</span></span>|<span data-ttu-id="6aed8-211">String</span><span class="sxs-lookup"><span data-stu-id="6aed8-211">String</span></span>|<span data-ttu-id="6aed8-212">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="6aed8-212">The name of the main Lob application file.</span></span> <span data-ttu-id="6aed8-213">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6aed8-214">size</span><span class="sxs-lookup"><span data-stu-id="6aed8-214">size</span></span>|<span data-ttu-id="6aed8-215">Int64</span><span class="sxs-lookup"><span data-stu-id="6aed8-215">Int64</span></span>|<span data-ttu-id="6aed8-216">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="6aed8-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="6aed8-217">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="6aed8-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6aed8-218">commandLine</span><span class="sxs-lookup"><span data-stu-id="6aed8-218">commandLine</span></span>|<span data-ttu-id="6aed8-219">String</span><span class="sxs-lookup"><span data-stu-id="6aed8-219">String</span></span>|<span data-ttu-id="6aed8-220">Командная строка.</span><span class="sxs-lookup"><span data-stu-id="6aed8-220">The command line.</span></span>|
|<span data-ttu-id="6aed8-221">productCode</span><span class="sxs-lookup"><span data-stu-id="6aed8-221">productCode</span></span>|<span data-ttu-id="6aed8-222">String</span><span class="sxs-lookup"><span data-stu-id="6aed8-222">String</span></span>|<span data-ttu-id="6aed8-223">Код продукта.</span><span class="sxs-lookup"><span data-stu-id="6aed8-223">The product code.</span></span>|
|<span data-ttu-id="6aed8-224">productVersion</span><span class="sxs-lookup"><span data-stu-id="6aed8-224">productVersion</span></span>|<span data-ttu-id="6aed8-225">String</span><span class="sxs-lookup"><span data-stu-id="6aed8-225">String</span></span>|<span data-ttu-id="6aed8-226">Версия бизнес-приложения, к которому применяется MSI Windows Mobile.</span><span class="sxs-lookup"><span data-stu-id="6aed8-226">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="6aed8-227">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="6aed8-227">ignoreVersionDetection</span></span>|<span data-ttu-id="6aed8-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aed8-228">Boolean</span></span>|<span data-ttu-id="6aed8-229">Логическое значение, позволяющее разрешить или запретить поиск установленного приложения по его версии.</span><span class="sxs-lookup"><span data-stu-id="6aed8-229">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="6aed8-230">Задайте значение true для бизнес-приложений MSI для Windows Mobile с функцией самостоятельного обновления.</span><span class="sxs-lookup"><span data-stu-id="6aed8-230">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="6aed8-231">identityVersion</span><span class="sxs-lookup"><span data-stu-id="6aed8-231">identityVersion</span></span>|<span data-ttu-id="6aed8-232">String</span><span class="sxs-lookup"><span data-stu-id="6aed8-232">String</span></span>|<span data-ttu-id="6aed8-233">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="6aed8-233">The identity version.</span></span>|
|<span data-ttu-id="6aed8-234">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="6aed8-234">useDeviceContext</span></span>|<span data-ttu-id="6aed8-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aed8-235">Boolean</span></span>|<span data-ttu-id="6aed8-236">Указывает, следует ли установить MSI с двойным режимом в контексте устройства.</span><span class="sxs-lookup"><span data-stu-id="6aed8-236">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="6aed8-237">Если задано значение true, приложение будет установлено для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="6aed8-237">If true, app will be installed for all users.</span></span> <span data-ttu-id="6aed8-238">Если задано значение false, приложение будет установлено для каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="6aed8-238">If false, app will be installed per-user.</span></span> <span data-ttu-id="6aed8-239">Если значение равно null, служба будет использовать стандартный контекст установки пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="6aed8-239">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="6aed8-240">В случае с двойным режимом MSI это значение по умолчанию будет иметь значение "на пользователя".</span><span class="sxs-lookup"><span data-stu-id="6aed8-240">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="6aed8-241">Не может быть задано для приложений с несдвоенным режимом.</span><span class="sxs-lookup"><span data-stu-id="6aed8-241">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="6aed8-242">После первоначального создания приложения его невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="6aed8-242">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="6aed8-243">Ответ</span><span class="sxs-lookup"><span data-stu-id="6aed8-243">Response</span></span>
<span data-ttu-id="6aed8-244">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6aed8-244">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aed8-245">Пример</span><span class="sxs-lookup"><span data-stu-id="6aed8-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="6aed8-246">Запрос</span><span class="sxs-lookup"><span data-stu-id="6aed8-246">Request</span></span>
<span data-ttu-id="6aed8-247">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6aed8-247">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6aed8-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="6aed8-248">Response</span></span>
<span data-ttu-id="6aed8-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6aed8-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





