---
title: тип ресурса riskyServicePrincipal
description: 'Представляет идентификаторы рабочей нагрузки Azure AD, которые находятся под угрозой, включая риски для приложений, директоров служб и управляемых удостоверений. '
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ad89892a3cb33bb182a7df1a2e12d9355c2178b0
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723741"
---
# <a name="riskyserviceprincipal-resource-type"></a>тип ресурса riskyServicePrincipal

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет принципы служб Azure AD, которые находятся в опасности. Azure AD непрерывно оценивает основной риск службы на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем директорам службы риска в клиенте Azure AD.

Наследует [от сущности](../resources/entity.md).

>**Примечание:** Использование API riskyServicePrincipal требует Azure AD Premium P2 лицензии.

## <a name="methods"></a>Методы

| Метод                                                                                      | Тип возвращаемых данных                                                                        | Описание                                                     |
| :------------------------------------------------------------------------------------------ | :--------------------------------------------------------------------------------- | :-------------------------------------------------------------- |
| [Список рискованныхServicePrincipals](../api/identityprotectionroot-list-riskyserviceprincipals.md) | [коллекция riskyServicePrincipal](../resources/riskyserviceprincipal.md)          | Список рискованных директоров служб и их свойств риска.        |
| [Get riskyServicePrincipal](../api/riskyserviceprincipal-get.md)                            | [riskyServicePrincipal](../resources/riskyserviceprincipal.md)                     | Получите определенную главу риск-службы и ее свойства риска. |
| [увольнение](../api/riskyserviceprincipal-dismiss.md)                                          | Отсутствует                                                                               | Отклоняй риск, связанный с риском для директора службы.                  |
| [confirmCompromised](../api/riskyserviceprincipal-confirmcompromised.md)                    | Отсутствует                                                                               | Подтвердит, что рисковая руководитель службы скомпрометирована.               |
| [История списка](../api/riskyserviceprincipal-list-history.md)                                | [коллекция riskyServicePrincipalHistoryItem](riskyserviceprincipalhistoryitem.md) | Получите историю рисков для директора службы Azure AD.          |

## <a name="properties"></a>Свойства

| Свойство                | Тип           | Описание                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| :---------------------- | :------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| accountEnabled          | Логический        | Значение `true`, если учетная запись субъекта-службы включена. В противном случае используется значение `false`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| appId                   | String         | Глобальный уникальный идентификатор для связанного приложения (его **свойства appId** ), если таково.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| displayName             | String         | Отображаемое имя для субъекта-службы.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| id                      | String         | Уникальный идентификатор, присвоенный директору службы в опасности. Наследуется от [сущности](../resources/entity.md).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| isProcessing            | Boolean        | Указывает, обрабатывает ли Azure AD в настоящее время рискованное состояние директора службы.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| riskDetail              | riskDetail     | Сведения об обнаружении риска. <br>**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Клиенты P1 будут возвращены `hidden`. <br/>Возможные значения: `none`, , `userPerformedSecuredPasswordChange``adminGeneratedTemporaryPassword`, , `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `adminDismissedAllRiskForServicePrincipal``adminConfirmedServicePrincipalCompromised``unknownFutureValue``hidden``adminDismissedAllRiskForUser``adminConfirmedUserCompromised``aiConfirmedSigninSafe``userPassedMFADrivenByRiskBasedPolicy``adminConfirmedSigninCompromised`. Обратите внимание, что для `Prefer: include-unknown-enum-members` получения следующего значения (ы) [](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)`adminConfirmedServicePrincipalCompromised` `adminDismissedAllRiskForServicePrincipal`в этом развиваемом переуме. |
| riskLastUpdatedDateTime | DateTimeOffset | Дата и время последнего обновления состояния риска. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, полночь UTC на 1 января 2021 года .`2021-01-01T00:00:00Z` Поддерживает `$filter` (`eq`).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| riskLevel               | riskLevel      | Уровень обнаруженного удостоверения рискованной рабочей нагрузки. Допустимые значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. Поддерживает `$filter` (`eq`).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| riskState               | riskState      | Состояние риска директора службы. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| servicePrincipalType    | Строка         | Определяет, представляет ли директор службы `Application`устаревшее или устаревшее `ManagedIdentity`приложение(`socialIdp`). Это задаваемо Azure AD внутренне и наследуется от [servicePrincipal](../resources/servicePrincipal.md).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |

## <a name="relationships"></a>Связи

| Связь | Тип                                                                               | Описание                                                 |
| :----------- | :--------------------------------------------------------------------------------- | :---------------------------------------------------------- |
| история      | [коллекция riskyServicePrincipalHistoryItem](riskyserviceprincipalhistoryitem.md) | Представляет историю рисков для директоров служб Azure AD. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyServicePrincipal",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.riskyServicePrincipal",
  "id": "String (identifier)",
  "accountEnabled": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "displayName": "String",
  "appId": "String",
  "servicePrincipalType": "String"
}
```
