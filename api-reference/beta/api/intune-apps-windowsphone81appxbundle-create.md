---
title: Создание windowsPhone81AppXBundle
description: Создание нового объекта windowsPhone81AppXBundle.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c660e7a211fae6ea4f1a180b4b1db75af644f9a9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401945"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="e81a3-103">Создание windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="e81a3-103">Create windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="e81a3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e81a3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e81a3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e81a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e81a3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e81a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e81a3-107">Создание нового объекта [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="e81a3-107">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e81a3-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="e81a3-108">Prerequisites</span></span>
<span data-ttu-id="e81a3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e81a3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e81a3-111">Permission type</span></span>|<span data-ttu-id="e81a3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e81a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e81a3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e81a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e81a3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e81a3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e81a3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e81a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e81a3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e81a3-116">Not supported.</span></span>|
|<span data-ttu-id="e81a3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e81a3-117">Application</span></span>|<span data-ttu-id="e81a3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e81a3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e81a3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e81a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e81a3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e81a3-120">Request headers</span></span>
|<span data-ttu-id="e81a3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e81a3-121">Header</span></span>|<span data-ttu-id="e81a3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e81a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e81a3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e81a3-123">Authorization</span></span>|<span data-ttu-id="e81a3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e81a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e81a3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e81a3-125">Accept</span></span>|<span data-ttu-id="e81a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e81a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e81a3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e81a3-127">Request body</span></span>
<span data-ttu-id="e81a3-128">В тексте запроса укажите представление JSON для объекта windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="e81a3-128">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="e81a3-129">В следующей таблице показаны свойства, которые необходимы для создания windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="e81a3-129">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="e81a3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e81a3-130">Property</span></span>|<span data-ttu-id="e81a3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e81a3-131">Type</span></span>|<span data-ttu-id="e81a3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e81a3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e81a3-133">id</span><span class="sxs-lookup"><span data-stu-id="e81a3-133">id</span></span>|<span data-ttu-id="e81a3-134">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-134">String</span></span>|<span data-ttu-id="e81a3-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e81a3-135">Key of the entity.</span></span> <span data-ttu-id="e81a3-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81a3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e81a3-137">displayName</span></span>|<span data-ttu-id="e81a3-138">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-138">String</span></span>|<span data-ttu-id="e81a3-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="e81a3-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e81a3-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81a3-141">description</span><span class="sxs-lookup"><span data-stu-id="e81a3-141">description</span></span>|<span data-ttu-id="e81a3-142">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-142">String</span></span>|<span data-ttu-id="e81a3-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="e81a3-143">The description of the app.</span></span> <span data-ttu-id="e81a3-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81a3-145">publisher</span><span class="sxs-lookup"><span data-stu-id="e81a3-145">publisher</span></span>|<span data-ttu-id="e81a3-146">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-146">String</span></span>|<span data-ttu-id="e81a3-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="e81a3-147">The publisher of the app.</span></span> <span data-ttu-id="e81a3-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81a3-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e81a3-149">largeIcon</span></span>|[<span data-ttu-id="e81a3-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e81a3-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e81a3-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="e81a3-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e81a3-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81a3-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e81a3-153">createdDateTime</span></span>|<span data-ttu-id="e81a3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e81a3-154">DateTimeOffset</span></span>|<span data-ttu-id="e81a3-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e81a3-155">The date and time the app was created.</span></span> <span data-ttu-id="e81a3-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81a3-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e81a3-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e81a3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e81a3-158">DateTimeOffset</span></span>|<span data-ttu-id="e81a3-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="e81a3-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e81a3-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81a3-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e81a3-161">isFeatured</span></span>|<span data-ttu-id="e81a3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e81a3-162">Boolean</span></span>|<span data-ttu-id="e81a3-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81a3-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e81a3-164">privacyInformationUrl</span></span>|<span data-ttu-id="e81a3-165">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-165">String</span></span>|<span data-ttu-id="e81a3-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="e81a3-166">The privacy statement Url.</span></span> <span data-ttu-id="e81a3-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81a3-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e81a3-168">informationUrl</span></span>|<span data-ttu-id="e81a3-169">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-169">String</span></span>|<span data-ttu-id="e81a3-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="e81a3-170">The more information Url.</span></span> <span data-ttu-id="e81a3-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81a3-172">owner</span><span class="sxs-lookup"><span data-stu-id="e81a3-172">owner</span></span>|<span data-ttu-id="e81a3-173">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-173">String</span></span>|<span data-ttu-id="e81a3-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="e81a3-174">The owner of the app.</span></span> <span data-ttu-id="e81a3-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81a3-176">developer</span><span class="sxs-lookup"><span data-stu-id="e81a3-176">developer</span></span>|<span data-ttu-id="e81a3-177">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-177">String</span></span>|<span data-ttu-id="e81a3-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="e81a3-178">The developer of the app.</span></span> <span data-ttu-id="e81a3-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81a3-180">notes</span><span class="sxs-lookup"><span data-stu-id="e81a3-180">notes</span></span>|<span data-ttu-id="e81a3-181">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-181">String</span></span>|<span data-ttu-id="e81a3-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="e81a3-182">Notes for the app.</span></span> <span data-ttu-id="e81a3-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81a3-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e81a3-184">uploadState</span></span>|<span data-ttu-id="e81a3-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e81a3-185">Int32</span></span>|<span data-ttu-id="e81a3-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="e81a3-186">The upload state.</span></span> <span data-ttu-id="e81a3-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81a3-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="e81a3-188">publishingState</span></span>|[<span data-ttu-id="e81a3-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e81a3-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e81a3-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="e81a3-190">The publishing state for the app.</span></span> <span data-ttu-id="e81a3-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="e81a3-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e81a3-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e81a3-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e81a3-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e81a3-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e81a3-194">isAssigned</span></span>|<span data-ttu-id="e81a3-195">Логический</span><span class="sxs-lookup"><span data-stu-id="e81a3-195">Boolean</span></span>|<span data-ttu-id="e81a3-196">Значение, указывающее, назначена ли приложение по крайней мере одной группы.</span><span class="sxs-lookup"><span data-stu-id="e81a3-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e81a3-197">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81a3-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e81a3-198">roleScopeTagIds</span></span>|<span data-ttu-id="e81a3-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e81a3-199">String collection</span></span>|<span data-ttu-id="e81a3-200">Список идентификаторов тег области для данного мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e81a3-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e81a3-201">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e81a3-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e81a3-202">committedContentVersion</span></span>|<span data-ttu-id="e81a3-203">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-203">String</span></span>|<span data-ttu-id="e81a3-204">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="e81a3-204">The internal committed content version.</span></span> <span data-ttu-id="e81a3-205">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e81a3-206">fileName</span><span class="sxs-lookup"><span data-stu-id="e81a3-206">fileName</span></span>|<span data-ttu-id="e81a3-207">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-207">String</span></span>|<span data-ttu-id="e81a3-208">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="e81a3-208">The name of the main Lob application file.</span></span> <span data-ttu-id="e81a3-209">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e81a3-210">size</span><span class="sxs-lookup"><span data-stu-id="e81a3-210">size</span></span>|<span data-ttu-id="e81a3-211">Int64</span><span class="sxs-lookup"><span data-stu-id="e81a3-211">Int64</span></span>|<span data-ttu-id="e81a3-212">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="e81a3-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="e81a3-213">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e81a3-214">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="e81a3-214">applicableArchitectures</span></span>|[<span data-ttu-id="e81a3-215">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="e81a3-215">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="e81a3-216">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="e81a3-216">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="e81a3-217">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="e81a3-217">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="e81a3-218">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="e81a3-218">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="e81a3-219">identityName</span><span class="sxs-lookup"><span data-stu-id="e81a3-219">identityName</span></span>|<span data-ttu-id="e81a3-220">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-220">String</span></span>|<span data-ttu-id="e81a3-221">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e81a3-221">The Identity Name.</span></span> <span data-ttu-id="e81a3-222">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="e81a3-222">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="e81a3-223">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="e81a3-223">identityPublisherHash</span></span>|<span data-ttu-id="e81a3-224">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-224">String</span></span>|<span data-ttu-id="e81a3-225">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="e81a3-225">The Identity Publisher Hash.</span></span> <span data-ttu-id="e81a3-226">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="e81a3-226">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="e81a3-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e81a3-227">identityResourceIdentifier</span></span>|<span data-ttu-id="e81a3-228">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-228">String</span></span>|<span data-ttu-id="e81a3-229">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="e81a3-229">The Identity Resource Identifier.</span></span> <span data-ttu-id="e81a3-230">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="e81a3-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="e81a3-231">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e81a3-231">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e81a3-232">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e81a3-232">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="e81a3-233">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="e81a3-233">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="e81a3-234">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="e81a3-234">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="e81a3-235">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="e81a3-235">phoneProductIdentifier</span></span>|<span data-ttu-id="e81a3-236">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-236">String</span></span>|<span data-ttu-id="e81a3-237">Идентификатор продукта телефона.</span><span class="sxs-lookup"><span data-stu-id="e81a3-237">The Phone Product Identifier.</span></span> <span data-ttu-id="e81a3-238">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="e81a3-238">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="e81a3-239">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="e81a3-239">phonePublisherId</span></span>|<span data-ttu-id="e81a3-240">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-240">String</span></span>|<span data-ttu-id="e81a3-241">Идентификатор издателя телефона наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="e81a3-241">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="e81a3-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e81a3-242">identityVersion</span></span>|<span data-ttu-id="e81a3-243">String</span><span class="sxs-lookup"><span data-stu-id="e81a3-243">String</span></span>|<span data-ttu-id="e81a3-244">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e81a3-244">The identity version.</span></span> <span data-ttu-id="e81a3-245">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="e81a3-245">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="e81a3-246">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="e81a3-246">appXPackageInformationList</span></span>|<span data-ttu-id="e81a3-247">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e81a3-247">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="e81a3-248">Список AppX сведения о пакете.</span><span class="sxs-lookup"><span data-stu-id="e81a3-248">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="e81a3-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="e81a3-249">Response</span></span>
<span data-ttu-id="e81a3-250">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e81a3-250">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e81a3-251">Пример</span><span class="sxs-lookup"><span data-stu-id="e81a3-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="e81a3-252">Запрос</span><span class="sxs-lookup"><span data-stu-id="e81a3-252">Request</span></span>
<span data-ttu-id="e81a3-253">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e81a3-253">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2184

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

### <a name="response"></a><span data-ttu-id="e81a3-254">Отклик</span><span class="sxs-lookup"><span data-stu-id="e81a3-254">Response</span></span>
<span data-ttu-id="e81a3-p129">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e81a3-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2356

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




