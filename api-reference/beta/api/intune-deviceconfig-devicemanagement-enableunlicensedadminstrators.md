---
title: enableUnlicensedAdminstrators action
description: После включения пользователям, назначенным администраторами с помощью членов назначения ролей, больше не потребуется назначенная лицензия Intune. Для каждой группы безопасности AAD в назначении ролей может быть ограничено 350 нелицензионных прямых членов, но при необходимости для поддержки более 350 нелицензионных администраторов можно назначить несколько групп безопасности AAD. Лицензированные администраторы будут продолжать функционировать как есть в том, что транзитные членства применяются и не подлежат ограничению в 350 членов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 149c14aab5672939174799791f6a4e0af970419d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128028"
---
# <a name="enableunlicensedadminstrators-action"></a>enableUnlicensedAdminstrators action

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

После включения пользователям, назначенным администраторами с помощью членов назначения ролей, больше не потребуется назначенная лицензия Intune. Для каждой группы безопасности AAD в назначении ролей может быть ограничено 350 нелицензионных прямых членов, но при необходимости для поддержки более 350 нелицензионных администраторов можно назначить несколько групп безопасности AAD. Лицензированные администраторы будут продолжать функционировать как есть в том, что транзитные членства применяются и не подлежат ограничению в 350 членов.

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableUnlicensedAdminstrators
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableUnlicensedAdminstrators
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 204 No Content
```




